---
aliases: [Initiative Tracker Encounter Builder]
cover: 
description: "Learn how to access and use the Encounter Builder feature in Initiative Tracker."
image: 
permalink: initiative/encounter-builder
publish: true
tags: [initiative/Encounters/Builder]
---

Initiative Tracker also features a comprehensive Encounter Builder. The encounter builder is used to look at the bestiary in its entirety to plan out the perfect tor- I mean, *challenge*, for your players. 

>[!screenshot]- Encounter Builder Pre Remake
> ![encounter-builder](https://github.com/javalent/initiative-tracker/blob/main/publish/images/encounter-builder/encounter-builder.png?raw=true)

## Accessing Encounter Builder

There are currently two ways to access the encounter builder. 

***Way of the Ribbon***:

1. On the lefthand sidebar ribbon, look for the hammer icon.
2. Click the Hammer Icon.
![float-right](https://github.com/javalent/initiative-tracker/blob/main/publish/images/encounter-builder/IT-Open-Encounter-Builder.png?raw=true)

***Way of the Hotkey***:

1.  Open Obsidian Settings and navigate to Hotkeys.
2.  Filter the Hotkeys list by the word `Encounter`.
3.  Set the option `Initiative Tracker: Open Encounter Builder` to the hotkey of your choice.
4.  Exit settings.
5.  Try your hotkey. The Encounter Builder tab should open in the same place your notes do.

***Way of the Command Palette***:

1.  Enable the Core Plugin Command Palette if it isn't already enabled in Obsidian Settings, then exit settings.
2.  Press `Ctrl/Cmd + P` to open the command palette. Alternatively, you may be able to open it from the left-hand ribbon.
3.  In the command palette search bar, type `Encounter`
4.  Select the option `Initiative Tracker: Open Encounter Builder`.
5.  The Encounter Builder tab should open in the same place your notes do.

## Encounter Builder View

### Players

In the Encounter Builder, the Players section allows you to optionally add unnamed players of a certain level. These help in difficulty calculation and also allow you to create empty player entries that can be edited and added formally later on.

Here are the details of the Players section:

![Players in Encounter Builder](https://github.com/javalent/initiative-tracker/blob/main/publish/images/encounter-builder/encounter-builder-players.png?raw=true)


1. Number of players at a particular level
2.  Level of all players in the group
3.  Remove a player group
4.  Add a player group

### Experience

The experience section of the encounter builder helps you determine the difficulty of the encounter by comparing the level of the creatures with that of the player characters.

![Experience](https://github.com/javalent/initiative-tracker/blob/main/publish/images/encounter-builder/encounter-builder-experience.png?raw=true)

1. This section shows the calculated experience for the encounter, based on the challenge rating of the selected creatures and the number of player characters.
2.  You can also see how much experience the players' group is expected to earn in a day, according to their level.

### The Headers

The Encounter headers consist of the section that displays the selected creatures, as well as the standard encounter launch, save, and export buttons.

![Headers](https://github.com/javalent/initiative-tracker/blob/main/publish/images/encounter-builder/encounter-builder-top.png?raw=true)

1. This is the list of selected monsters.
2.  From Left to Right, the buttons are:
    1.  Start Encounter Button
    2.  Save Encounter Button
    3.  Load Encounter Button
    4.  Erase (Reset Builder)

### Filters in Depth

![Filters in Depth](https://github.com/javalent/initiative-tracker/blob/main/publish/images/encounter-builder/dynamic-filtering.png?raw=true)


With the encounter builder's filters, you can narrow down your search based on various criteria, including:

1.  Creature name
2.  Creature size
3.  Creature type
4.  Creature alignment
5.  Maximum level

You can also further enhance your search by: 

6. Showing/hiding extra filters
7.  Resetting the filters
8.  Filter settings:
    1.  Edit headers and layout: brings up a modal to customize the layout
    2.  Export filter settings (filter, header, and collapse state)
    3.  Import filter settings (also, filter, header, and collapse state)

## Using the Encounter Builder

> [!screenshot]- Filtering in Action
> ![Filter Evil](https://github.com/javalent/initiative-tracker/blob/main/publish/images/encounter-builder/filter-alignment.png?raw=true)

 Typing the word 'evil' brings up any alignment with the word evil in it.

### Dynamic Filtering

The encounter builder's filters are designed to extract data from the entries in the relevant field, allowing you to easily locate specific items regardless of their names.

> [!screenshot]- Image of Filters Available for Type
> ![Filtering](https://github.com/javalent/initiative-tracker/blob/main/publish/images/encounter-builder/pulling-from-fields.png?raw=true)

### Editing Filters and Headers

The encounter builder has a feature to edit the layout of headers for filtering, similar to the [[Fantasy Statblocks]] plugin.

> [!screenshot]- Gif of the Layout Editor
> ![Editor Filtering](https://github.com/javalent/initiative-tracker/blob/main/publish/gifs/encounter-builder.gif?raw=true)

