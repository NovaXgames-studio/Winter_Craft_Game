# Wintercraft Reborn

Official game package for **Wintercraft Reborn** on Luanti/Minetest-compatible engines.

This repository contains the **game only** (`wintercraft_game`).

## Features

- Survival and crafting progression
- Expanded mobs and creatures
- Nether content and world expansion
- Decorative blocks and furniture systems
- HUD, hunger, inventory, and utility gameplay modules

## Requirements

- Luanti or Minetest-compatible engine installed
- A valid `games/` directory in your engine user data folder

## Installation

1. Close Luanti/Minetest.
2. Copy this repository folder as:
   - Windows (Luanti): `%APPDATA%\\Luanti\\games\\wintercraft_game`
   - Windows (Minetest): `%APPDATA%\\Minetest\\games\\wintercraft_game`
3. Launch the engine.
4. Create a new world and select **Winter Craft** as the game.

## Included Modules

The `mods/` folder includes core gameplay systems and content packs such as:

- Core: `default`, `farming`, `doors`, `stairs`, `wool`, `bucket`, `boats`, `carts`
- Creatures: `mobs_redo`, `mobs_animal`, `mobs_monster`, `mobs_npc`, `mobs_humans`, `mob_horse`, `dmobs`
- World and tools: `nether`, `fire`, `flowers`, `tnt`, `xdecor`, `worldedit`, `worldedit_commands`
- Interface and progression: `hud`, `hunger`, `creative`, `craftguide`, `sfinv`, `give_initial_stuff`

## Repository Layout

- `game.conf`: game metadata
- `mods/`: gameplay modules
- `menu/`: menu assets and definitions
- `minetest.conf.example`: optional configuration template
- `LICENSE.txt`: license information

## Development

Contributions are welcome for:

- Bug fixes
- Balancing and gameplay updates
- Content expansion
- Performance and compatibility improvements

## License

See [LICENSE.txt](LICENSE.txt).
