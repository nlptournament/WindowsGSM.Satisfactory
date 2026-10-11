# WindowsGSM.Satisfactory.Unreal5
WindowsGSM plugin that provides Satisfactory Dedicated server support for the latest release. 
This was forked from https://github.com/werewolf2150/WindowsGSM.Satisfactory and recoded to work for Unreal 5 for the 1.0 release of Satisfactory

# Requirements
WindowsGSM >= 1.23.1

# The Game

- Game
https://store.steampowered.com/app/526870/Satisfactory/

- Dedicated server
https://store.steampowered.com/app/1690800/Satisfactory_Survival/

# Installation

1. Download the latest release: [WindowsGSM.Satisfactory.Unreal5](https://github.com/Kavex/WindowsGSM.Satisfactory.Unreal5/archive/refs/heads/main.zip)
2. Move **Satisfactory.cs** folder to plugins folder
3. Click **[RELOAD PLUGINS]** button or restart WindowsGSM

# Ports

| Port | Protocol | Purpose |
| ---- | -------- | ------- |
| 7777 | TCP + UDP | Game port, also the HTTPS API (`/api/v1`) |
| 8888 | TCP | Messaging (reliable) port, set in the WindowsGSM **Query Port** field |

The old query port (15777) and beacon port (15000) are no longer used. Open the ports above in your firewall.

# Features

- Launches with `-Port`, `-ReliablePort` and `-ExternalReliablePort`
- Max players is applied through `-ini` overrides
- Server IP is passed as `-multihome` when set
- No A2S query (the server no longer supports it)

# Settings

1. Open game and connect
2. First connection initialise parameters
3. manage server directly in game.
