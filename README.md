# Desmume For Pokemon - Download from Releases >>>>

## Features

This is a fork of Desmume that is intended to enhance the Pokemon nuzlocking experience for both Windows and Macos

- automatic trainer battle logging and fragsheet tracking
- allows automatic syncing of your party/box via websockets
- an in-emulator pokemon editor that allows for pre-damage/pre-status/exp edging and more
- in game time selection to easily access time gated events/encounter tables 


## Setup 

1. Open Rom in DeSmuMe.
2. Select Rom Name in the Poketools Menu
3. All Features should be automatically availalbe under the Tools menubar


## Battle Logging
- All logs are output to a `dumps` folder in the same folder as whereever you are keeping your Battery/ save files
- Every time you start a new run with a new Trainer ID, a new `Attempt` folder is created 
- Trainer battles are logged automatically.
- Wild battles are skipped for battle log sessions.
- Logging starts when a trainer battle is detected.
- Logging stops automatically when the battle ends.

# Desmume For Nuzlockers Guide

Below is an overview of Desmume's Pokemon Specific Functions

## Poketools

There is now a new Poketools menu next to the tools menu
<img width="273" height="272" alt="Screenshot 2026-04-10 at 1 00 57 PM" src="https://github.com/user-attachments/assets/6431d338-f500-48d9-86c0-e8db3b0c1366" />

For all feature, you must make sure you have selected the correct Pokemon Game in `Select Pokemon Game` for them to work properly

### HTTP API Features

When a supported Pokemon game is running if you click `Enable HTTP API` desmume will open a connection and start serving your party/box data, and battle log data for other apps like damage calculators to read. 

Note: If this is causing noticeable lag, you can disable it, battle logs will still be recorded, and your party/box export can still be synced to the damage calc via your Copy Paste Clipboard

### Clipboard Functions

You can click `Copy Pokemon Export to Clipboard` to copy your current Party and Box (except last box) to your clipboard. You can also set this  via a hotkey. 

When you click `Sync` in Dynamic Calc, the calc will first check if there is a http connection open, and if not, it will check your clipboard for a showdown paste so it should function the same as the HTTP sync.

By default, your clipboard will be autoupdated every 10 seconds while you're not in battle, but this autoupdate can be toggled off, or have the timing adjusted. 
<img width="234" height="188" alt="Screenshot 2026-04-10 at 1 01 13 PM" src="https://github.com/user-attachments/assets/f762e9b7-2ba2-4581-8c70-fbf70b8614d3" />

### Pokemon HTTP Maintenance

These settings control how often desmume will try to refresh your http connection if it is enabled, and how often it will refresh your copy/paste clipboard. 

Health check means how often it checks to see if the connection is still running

Idle Refresh refers to how often it will refresh the connection no matter what.

Enable Clipboard auto copy lets you turn on/off auto updating your copy paste clipboard with pokemon export.

Clipboard Auto copy interval lets you control how often the above happens. 

## Editors

There are two separate editors in Desmume one for full editing access to both your Party/Box and one that is a convenience editor just for your party that loads faster. Both editors can be accessed through the Poketools menu or by configurable hotkey

### Party Box Editor 
<img width="909" height="586" alt="Screenshot 2026-04-10 at 1 13 55 PM" src="https://github.com/user-attachments/assets/17169072-cb0c-4ac6-88c5-4f3b51acb61b" />

Edits that manipulate pokemon battle stats are currently disabled in the party editor so as to not affect your pokemon stats in certain romhacks. To edit things like level, and moves it is recommended to edit in the PC box.

### Party Editor

<img width="1035" height="374" alt="Screenshot 2026-04-10 at 1 15 36 PM" src="https://github.com/user-attachments/assets/a6b5db50-22b8-4b2b-b5d4-70b81905517a" />

This is a convenience editor meant for quick pre status/damage



## Dynamic Calc Pairing 

This script is built to work with **Dynamic Calc** fragsheet tools.

While a supported game is loaded in Desmume click `Sync` below the import box to import your currenty party/box.
<img width="293" height="152" alt="Screenshot 2026-03-19 at 2 08 40 PM" src="https://github.com/user-attachments/assets/22ee8836-10aa-4def-a6a6-ae7252a563aa" />

While on the fragsheet page, click `Sync` to import your current battle history 
<img width="1287" height="952" alt="Screenshot 2026-03-19 at 2 08 28 PM" src="https://github.com/user-attachments/assets/15aa4652-dc6c-4553-975b-00b994561492" />


### Troubleshooting

Report bugs in the [discord](https://discord.gg/HCXJFBANV2)

### Src

https://github.com/hzla/desmume-crossplatform-build
