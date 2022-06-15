![](https://img.shields.io/badge/Foundry-v9-informational)
![Latest Release Download Count](https://img.shields.io/github/downloads/colinbate/rolltable-requester/latest/module.zip)

# Rolltable Requester

Rolltables (or rollable tables, or random tables) are a great way to fuel ideas and add a bit of randomness to your games. They are often used ahead of time to set up a session or as part of world building. However they are also sometimes used directly within a game. The issue with rolling on a roll table in Foundry is that accessing them as players is awkward.

This module makes it easier to use rolltables during your game and involve your players. If you want to give your players Observer access to your tables so they can open them and roll on them, then you don't need this module. If you want then to be able to roll but not see the full list (or even the result), then this may be the module you are looking for. *waves hand like a Jedi*

## Features

Adds options to the context (right-click) menu of the rolltables:
- Make Roll
  - Performs the roll in public and displays the results to GM only.
- Request Named Roll
  - Displays a chat card with button asking a player to click it to roll on a the table which is named. When they click it, the roll happens just as with the 'Make Roll' option.
- Request Blind Roll
  - Displays the same chat card prompt, but without the name of the table.


Provides API access to making and requesting rolls above, so you can add them to macros.

If you give Limited access to a roll table to a player, they can access the 'Make Roll' option, providing a self service way for them to roll without being able to see the full list of options.

## API

The following functions are available:

```js
// Only option is setting { blind: true }.
RolltableRequester.requestRollById(tableId, opts);
RolltableRequester.requestRollByName(tableName, opts);

RolltableRequester.makeRollById(tableId);
RolltableRequester.makeRollByName(tableName);
```

## Changelog

See the Releases page for notes for each version.
