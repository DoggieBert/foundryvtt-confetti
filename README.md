# Confetti

![Latest Release Download Count](https://img.shields.io/badge/dynamic/json?label=Downloads@latest&query=assets%5B1%5D.download_count&url=https%3A%2F%2Fapi.github.com%2Frepos%2FElfFriend-DnD%2Ffoundryvtt-confetti%2Freleases%2Flatest)
![Forge Installs](https://img.shields.io/badge/dynamic/json?label=Forge%20Installs&query=package.installs&suffix=%25&url=https%3A%2F%2Fforge-vtt.com%2Fapi%2Fbazaar%2Fpackage%2Fgm-screen&colorB=4aa94a)
![Foundry Core Compatible Version](https://img.shields.io/badge/dynamic/json.svg?url=https%3A%2F%2Fraw.githubusercontent.com%2FElfFriend-DnD%2Ffoundryvtt-confetti%2Fmain%2Fsrc%2Fmodule.json&label=Foundry%20Version&query=$.compatibleCoreVersion&colorB=orange)
[![ko-fi](https://img.shields.io/badge/-buy%20me%20a%20coke-%23FF5E5B)](https://ko-fi.com/elffriend)


Everyone loves Confetti.

## Installation

Module JSON:

```
https://github.com/ElfFriend-DnD/foundryvtt-confetti/releases/latest/download/module.json
```

## Screenshots

![Demonstration of the GM Screen Grid with dnd5e content.](readme-img/dnd5e-demo.jpg)

## Configuration

| **Name**              | Description                                                                                                                                                |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Display as Drawer** | Defaults to True, set to false if you would like to use the GM Screen as a normal popup dialog or if you want to use the PopOut module with the GM Screen. |
| **Columns**           | Sets the number of columns in the grid.                                                                                                                    |
| **Rows**              | Sets the number of rows in the grid.                                                                                                                       |
| **Reset Grid**        | Saving with this checkbox checked will reset the grid (useful if you end up somehow causing it to fail to render).                                         |

Note that changing the grid dimensions after populating the grid might cause unexpected results, and odds are you will have to clear the grid and repopulate things.

## Compatibility

I'm honestly not sure how well this will play with modules that make changes to how journal articles or roll tables interact.

| **Name**                                                      |       Works        | Notes                                                                                                                                                                                                   |
| ------------------------------------------------------------- | :----------------: | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [OneJournal](https://gitlab.com/fvtt-modules-lab/one-journal) |        :x:         | Causes some unexpected oneJournal renders. Journal entries with html in them (tables in particular) don't seem to render. [Open MR](https://gitlab.com/fvtt-modules-lab/one-journal/-/merge_requests/2) |
| [MEME](https://github.com/Moerill/fvtt-markdown-editor)       | :heavy_check_mark: | Markdown Renders as expected.                                                                                                                                                                           |

## Known Issues

- The grid does not refresh automatically when settings are changed, click the "refresh" button.

## Acknowledgements

Bootstrapped with Nick East's [create-foundry-project](https://gitlab.com/foundry-projects/foundry-pc/create-foundry-project).

Mad props to the [League of Extraordinary FoundryVTT Developers](https://forums.forge-vtt.com/c/package-development/11) community which helped me figure out a lot.
