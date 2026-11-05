# Aethrix

A suite of plugins for [openac-rust](https://github.com/eriknihlen/openac-rust), the Asheron's Call client written in Rust. Each plugin does one job and runs on its own; plugins built to work together call each other through the client's plugin services.

This repository holds releases only. The source is private for now, and we intend to open-source it once the suite is feature complete.

## The plugins

| Plugin | What it does | Status |
|---|---|---|
| **Aethrix Vision** | Finds the objects and people you're watching for, marks them in the world with labels and gems, shows them on a HUD, and shades ground you can't walk on | First release coming |
| **Aethrix Combat** | Fights for you: melee, healing and stamina kits, walking to creatures, hunting dungeons and planned routes | In development |
| **Aethrix Atlas** | Maps, routes, waypoints and travel | Planned |
| **Aethrix Loot**, **Aethrix Buffs** | Judging and sorting loot; keeping buffs up | Planned |

Each plugin is released as soon as it's ready, starting small and growing.

## Installing

1. In the openac-rust launcher, open the plugin list and choose **Add from URL**.
2. Enter `https://github.com/davidc-smith/OpenAC-Aethrix`.
3. The launcher lists the suite's plugins that aren't installed yet. Pick one; it asks again for the rest until you cancel.
4. A new plugin is installed **disabled**. Enable it in the plugin list.

The launcher checks this repository for updates. Put a plugin on the **Beta** channel to be offered its pre-release versions too.

Every plugin needs launcher and client **0.1.11** or later. Older launchers don't see the suite's releases.

## Reporting a problem

Each plugin keeps its recent activity in memory while you play. When something goes wrong, run its report command, for example `/vision report`. It writes a file and says in chat where it is. Open an issue here with that file, what went wrong and about when.

## Releases

Each plugin has its own versions and tags, `wasm-<plugin id>-v<version>`, for example `wasm-rabiddee.aethrix-vision-v0.1.0`. The `wasm-index` release holds `plugins-index.json`, which points the launcher at each plugin's latest stable and beta release.
