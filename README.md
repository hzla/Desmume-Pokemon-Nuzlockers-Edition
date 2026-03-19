# Desmume For Pokemon

Current Supported Games:

- Pokemon Platinum (and platinum rom hacks)

## Features

This is a fork of Desmume that is intended to enhance the Pokemon nuzlocking experience for both Windows and Macos

- automatic trainer battle logging and fragsheet tracking
- allows automatic syncing of your party/box via websockets
- an in-emulator pokemon editor that allows for pre-damage/pre-status/exp edging and more 

It is designed to pair with the a **Dynamic Calc** calculator by giving the calc 

## Basic Setup (DeSmuMe)

1. Open Pokemon Platinum in DeSmuMe.
2. Load the Lua script (`Plat_Qol.lua`) through DeSmuMe's Lua scripting window.
3. Keep the script running while you play. If you need to restart your game, make sure you also restart the script, or just restart the script which will automatically also restart your game.


## Core Behavior (Battle Logging)

- Trainer battles are logged automatically.
- Wild battles are skipped for battle log sessions.
- Logging starts when a trainer battle is detected.
- Logging stops automatically when the battle ends.
- All logs are output to a `dumps` folder in the same folder as whereever you are keeping your Battery/ save files


### Editors

Under the Tools option in the Desmume menu you will find pokemon editors


## Dynamic Calc Pairing 

This script is built to work with **Dynamic Calc** fragsheet tools.

While a supported game is loaded in Desmume click `Sync` below the import box to import your currenty party/box


### Troubleshooting

Report bugs in the [discord](https://discord.gg/HCXJFBANV2)
