# Winter Craft Game (Luanti/Minetest)

This repository contains the extracted **game package only** for Winter Craft.

It does **not** contain the mobile engine binary (APK native engine).

## Project Scope

- Game name: `Winter Craft`
- Source package: Android app data extraction
- Repository content: `game.conf`, `mods/`, `menu/`, configs, and game assets
- Out of scope: engine binaries, launcher APK internals, account/network backend

## Current Status

- The game files are recovered and organized as a Luanti/Minetest game folder.
- Many mods load correctly on desktop Luanti/Minetest.
- Some features depend on mobile-specific engine APIs and may require patches.

## Included Gameplay Modules

Main module groups in `mods/` include:

- Core gameplay: `default`, `farming`, `doors`, `stairs`, `wool`, `bucket`, `boats`, `carts`
- Mobs: `mobs_redo`, `mobs_animal`, `mobs_monster`, `mobs_npc`, `mobs_humans`, `mob_horse`, `dmobs`
- World/features: `nether`, `tnt`, `fire`, `flowers`, `xdecor`, `worldedit`, `worldedit_commands`
- UI/systems: `hud`, `hunger`, `creative`, `craftguide`, `sfinv`, `give_initial_stuff`

## Install (Windows)

1. Close Luanti/Minetest.
2. Copy this folder into your games directory.
3. Use this final path:
   - Minetest: `%APPDATA%\Minetest\games\wintercraft_game`
   - Luanti: `%APPDATA%\Luanti\games\wintercraft_game`
4. Start the engine and select **Winter Craft** when creating a world.

Important:

- The folder name should stay `wintercraft_game` for predictable behavior.
- If your engine cannot see the game, verify `game.conf` is present in the root.

## Compatibility Notes

This game was built for a custom mobile environment. Upstream desktop engines may miss specific APIs.

Example:

- `minetest.register_on_shopaction` can be absent in stock builds, affecting shop callbacks.

If startup fails, read `debug.txt` and patch missing APIs/mod assumptions one by one.

## Legal / Credits

- Original game assets and branding belong to their respective owners.
- This repository is for preservation, interoperability testing, and modding research.
- See `LICENSE.txt` for bundled license terms where provided.

## Contribution

Pull requests are welcome for:

- Desktop compatibility fixes
- Missing API shims for Luanti/Minetest
- Bugfixes in extracted mods
- Documentation improvements
