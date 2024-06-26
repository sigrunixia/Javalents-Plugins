---
aliases: [Days and Weeks and Months and Years]
created: 2023-08-04
description: This page talks about modifying the day, week, month, and year
permalink: calendarium/styling
publish: true
tags: [Calendarium/Components]
updated: 2024-04-26
---

# Days and weeks and months and years

The code displayed on this page is Svelte. Svelte is a front-end wrapper for multiple code types, and Javalents' plugins use it heavily. Learn more about [Svelte at their website](https://svelte.dev/blog/write-less-code).

## Component bunching

### Week view

The Plugin generates the view of multiple days, using the Svelte code below

```svelte
<div class="week calendarium">
    {#if $displayWeeks}
        <span class="week-number">{weekNumber}</span>
    {/if}
    {#each week as day}
        <Day {...getMonth(day)} />
    {/each}
</div>
```

### Month view

A month is made up of multiple blocks of week components. This means any errors on the Week will transliterate to month. However, it also greatly increases uniformity of your calendar.

```svelte
{#if $viewState == ViewState.Year}
    <h4 class="calendarium month-header">{displayedMonth.name}</h4>
{/if}
<div
    class="calendarium month-container"
    class:full={$full}
>
    <Weekdays {year} {month} />
    <div class="calendarium month">
        {#each weekArray as week}
            <Week
                {month}
                {year}
                startingDay={week * $weekdays.length - $firstDay}
            />
        {/each}
    </div>
</div>
```

### Year view

A year is made up of multiple blocks of month components. This means any errors on the Week component will transliterate to the month component, which transliterate to your Year View. However, as mentioned, it also greatly increases uniformity *and speed* of your calendar.

```svelte
<div class="year-view">
    <div class="year" bind:this={yearContainer} use:focus class:full={$full}>
        {#each $monthArray as month, index}
            <div class="month-container" id={getIdForMonth(month.name)}>
                <Month year={$displaying.year} month={index} />
            </div>
        {/each}
    </div>
</div>
```