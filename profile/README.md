# GrangerMC

A Hypixel-style Minecraft minigame network — Velocity proxy + dynamically-scaled Paper servers,
orchestrated by [CloudNet v4](https://github.com/CloudNetService/CloudNet), with a shared
[LuckPerms](https://luckperms.net) rank hierarchy across the whole network. Built from source,
version-pinned, boot-tested end to end rather than assumed.

## Repos

| Repo | What it is |
|---|---|
| [`GrangerNetwork`](https://github.com/GrangerMC/GrangerNetwork) | Deployment/orchestration — Docker Compose, CloudNet templates, setup scripts, the bot test harness |
| [`granger-core`](https://github.com/GrangerMC/granger-core) | Shared base every backend server depends on — network-wide `/broadcast`, live game-state reporting, GUI/scoreboard/player-state/timing utilities |
| [`granger-proxy`](https://github.com/GrangerMC/granger-proxy) | `granger-core`'s Velocity-side companion — relays `/broadcast` to every connected player network-wide |
| [`granger-lobby`](https://github.com/GrangerMC/granger-lobby) | The lobby experience — void world, NPC server-selector, live sidebar, branded tab list |
| [`granger-minigame-core`](https://github.com/GrangerMC/granger-minigame-core) | Shared base every *minigame* depends on — join/countdown/start/end lifecycle, spectating, arena/map setup tooling |
| [`granger-web`](https://github.com/GrangerMC/granger-web) | Staff ops dashboard — live server list, start/stop/restart, rank management |

## Stack

Velocity · PaperMC · CloudNet v4 · LuckPerms · MariaDB · Redis · NamelessMC · Next.js
