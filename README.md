# WF Companion

An unofficial desktop companion for **Warframe** (Windows 10/11): your tradeable inventory with warframe.market prices, listings and status, a relic reward overlay, relic and ducat tools, mastery planning, and worldstate alerts with Discord/Telegram notifications.

**[Download the latest version](https://github.com/novicetinkerer/wf-companion-releases/releases/latest)** · [Website](https://novicetinkerer.github.io/wf-companion-releases/)

> [!WARNING]
> **This project was built with substantial help from AI.** Much of the code was written by an AI assistant (Claude, by Anthropic), directed, reviewed and tested by the author. It may contain mistakes. Use it at your own risk and report problems in [Issues](https://github.com/novicetinkerer/wf-companion-releases/issues).

> [!CAUTION]
> **Ban risk.** Inventory scans open the game process **read-only** (no writing, no injection) to read your account data. Similar tools are widely used, but no third-party tool that opens the game process can be guaranteed safe from anti-cheat or Digital Extremes' rules. Turn on **Safe mode** (first-run setup or Settings) to never touch the game process; everything except inventory scans keeps working.

## Features

- **Inventory**: prime & weapon parts, mods, arcanes and relics with average price, lowest sell / highest buy and your own listings; post and edit warframe.market orders from any item.
- **Relic reward overlay**: prices, ducats, owned parts (owned / needed for the set) and ★ wanted parts under each reward card.
- **Relics**: Radiant prices and run values, refine advice, Void Trace fodder, era filters, wanted-part highlights.
- **Wanted**: mark the prime parts you're after; relics that drop them are highlighted everywhere.
- **Mastery**: MR progress bar and "Next to master": what you can rank up, build now, craft, or get from relics you own.
- **Ducanator, Arcane Dissolution, Tracker** (currencies, Void Traces, relics opened per day), **Market** browser.
- **Alerts**: fissures, open-world cycles, Circuit, Baro, sorties; desktop, Discord and Telegram notifications; whisper notifications.
- Low RAM while you play: the window can close itself when Warframe starts; the tray app stays at ~15 MB.

## Install

1. Download `WF.Companion_<version>_x64-setup.exe` from the [latest release](https://github.com/novicetinkerer/wf-companion-releases/releases/latest) and run it.
2. Windows SmartScreen may warn because the installer isn't code-signed: **More info → Run anyway**.
3. The app updates itself: when a new version is out it asks you, and installs only when you're not playing.

Requirements for the relic overlay: Warframe in **Borderless Windowed**, and the **English (United States)** language pack (Windows text recognition). Settings → Relic overlay → *Check requirements* tests both.

## What it reads

| Feature | How | Touches the game process? |
|---|---|---|
| Inventory scan | Read-only memory read of your account data | Yes, read-only, a few seconds per scan (off in Safe mode) |
| Relic overlay | Screenshot of the game window + Windows OCR | No |
| Mission state, trades, whispers | Reads `EE.log` as a file | No |
| Prices, listings, status | warframe.market API | No |
| Alerts | Digital Extremes' public worldstate | No |

## License and source

GPL-3.0-or-later. The memory reader, warframe.market session handling and screen OCR are adapted from [FrameForge](https://github.com/WyrmStudios/FrameForge) (GPL-3.0). **The complete source code of each version is attached to its release** (`wf-companion-<version>-source.zip`).

Not affiliated with Digital Extremes or warframe.market. Warframe and its content are trademarks of Digital Extremes Ltd. Data: warframe.market, Digital Extremes public export, WFCD, warframe-public-export-plus, drops.warframestat.us.
