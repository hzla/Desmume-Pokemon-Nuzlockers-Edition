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
<img width="698" height="454" alt="Screenshot 2026-03-19 at 1 56 50 PM" src="https://github.com/user-attachments/assets/3115f58d-bf84-4c56-88b8-d4a0a85ae9ae" />
<img width="345" height="194" alt="Screenshot 2026-03-19 at 1 56 43 PM" src="https://github.com/user-attachments/assets/30ea9152-9045-4e4c-8bf1-630d3f18d2eb" />


## Dynamic Calc Pairing 

This script is built to work with **Dynamic Calc** fragsheet tools.

While a supported game is loaded in Desmume click `Sync` below the import box to import your currenty party/box.
<img width="293" height="152" alt="Screenshot 2026-03-19 at 2 08 40 PM" src="https://github.com/user-attachments/assets/22ee8836-10aa-4def-a6a6-ae7252a563aa" />

While on the fragsheet page, click `Sync` to import your current battle history 
<img width="1287" height="952" alt="Screenshot 2026-03-19 at 2 08 28 PM" src="https://github.com/user-attachments/assets/15aa4652-dc6c-4553-975b-00b994561492" />


### Troubleshooting

Report bugs in the [discord](https://discord.gg/HCXJFBANV2)
