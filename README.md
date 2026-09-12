<p align="center">
  <img src="Andys-Smart-Tool-Swapper-Hero-16x9-FINAL.png" alt="Andy's Smart Tool Swapper" width="100%">
</p>

# Andy's Smart Tool Swapper

**Not just the right tool — the right tool for the drop you want.**

Every other automatic tool switcher asks *what category of tool breaks this block?* This one asks *of everything you are carrying, which exact tool belongs in your hand for this exact block, given what you want out of it?* Diamond ore gets your Fortune pickaxe, a spawner gets Silk Touch, a pickaxe two hits from breaking gets skipped, and a 3×3 Hammer never gets equipped by surprise. Start breaking something and the right tool comes to hand; stop, and whatever you were holding comes straight back.

<p align="center">
  <img src="images/player-menu-1.png" alt="The SwapperControl settings menu open in game" width="700">
</p>

_Your personal settings, opened from a Stick renamed `SwapperControl` at an Anvil._

**Current release:** 0.2.3
**Download:** [Andys_Smart_Tool_Swapper_0.2.3.mcaddon](Andys_Smart_Tool_Swapper_0.2.3.mcaddon)
**SHA-256:** `8825B185895D69D18401A3B31FA3B16D4B94601D4A20A0E2CB8967483303E508`

Minecraft Bedrock **1.26.30 or newer** is required. Both the Behavior Pack and Resource Pack must be active — they depend on each other, so activating either activates the other. No cheats, commands, experimental gameplay toggles, or additional dependencies are required. Standard graphics and Vibrant Visuals are supported.

The complete player, user, and admin documentation is in the [GitHub Wiki](https://github.com/CharlesJGantt/Andys-Smart-Tool-Swapper/wiki).

## Features

- Automatic selection for pickaxes, axes, shovels, hoes, shears and melee weapons, including the blocks other switchers get wrong — sculk, sponge, hay, bamboo, muddy mangrove roots, nether stems, copper in every state, cobwebs, wool and leaves
- Fortune and Silk Touch treated as choices about the drop. By default a tool you deliberately picked up is never swapped away; Smart mode instead picks the enchantment each block deserves
- Returns your previous item when you stop — it borrows, it does not take over
- Follows what you *do*, not where you look. Once you start mining, the tool keeps up as the material changes without releasing the button
- Four selection strategies: Balanced, Fastest, Preserve Valuable Gear, Lowest Adequate Tier
- Three durability policies plus a safety floor that skips tools close to breaking
- Area tools such as Hammers are never auto-selected unless you switch them on
- Mark any individual tool Preferred or Never auto-select — the mark follows that exact item, not its type
- Teach Smart Tool Swapper registers custom tools from other add-ons
- Hold sneak to pause. Builder protection and Combat Lock keep it out of your way
- Per-player settings, a full operator menu, and complete dedicated-server console support
- **Adds no items or blocks of its own**

## Crafting Recipes

No Crafting Table recipes. Both menus open from a plain vanilla Stick renamed at an Anvil. The name is matched exactly, **including capital letters**.

### SwapperControl

Rename a **Stick** to `SwapperControl` at an Anvil. Opens your personal settings, the Mark-a-tool page, and the "Why did it pick that tool?" report. Any player may use one.

<p align="center">
  <img src="images/swappercontrol-anvil.png" alt="Renaming a Stick to SwapperControl at an Anvil" width="600">
</p>

### AdminSwapperControl

Rename a **Stick** to `AdminSwapperControl` at an Anvil. Opens the world settings and Teach Smart Tool Swapper. **Operators only** — anyone can rename a Stick, so the restriction is enforced when the menu opens, and a non-operator is told so in chat rather than left with an item that does nothing.

<p align="center">
  <img src="images/adminswappercontrol-anvil.png" alt="Renaming a Stick to AdminSwapperControl at an Anvil" width="600">
</p>

## Installation

### Windows, Android, iPhone, and iPad

1. Download [Andys_Smart_Tool_Swapper_0.2.3.mcaddon](Andys_Smart_Tool_Swapper_0.2.3.mcaddon).
2. Open it with Minecraft Bedrock and wait for both packs to import.
3. Create or edit a world.
4. Activate **Andy's Smart Tool Swapper [BP]** under Behavior Packs.
5. Confirm **Andy's Smart Tool Swapper [RP]** is active under Resource Packs.
6. Enter the world holding anything at all and start breaking a block — the right tool comes to hand immediately.

Back up an important world before installing or updating any add-on.

### Xbox, PlayStation, and Nintendo Switch

Import and activate the add-on on Windows or mobile, upload the prepared world to a Realm, and join that Realm from the console.

## How it works

1. **Start breaking a block.** A swap follows what you do, never where you look — glancing past a cow, a chest and a log on the way to the block you wanted changes nothing.
2. **Keep going.** The tool keeps up as the material changes: stone → gravel → dirt → log → stone, without releasing the button.
3. **Stop.** Whatever you were holding comes back within about half a second.
4. **Hold sneak** at any time to pause the swapper entirely. Release to resume.
5. **Rename a Stick** to `SwapperControl` to change any of it, or `AdminSwapperControl` if you are the world owner.

Every setting has a per-player version, and the world owner decides whether players may change their own. Dedicated servers configure everything from the console — `scriptevent andy_sts:help` lists all sixteen commands, and they are authorized by event source, so the console is never refused for the lack of a player behind it.

<p align="center">
  <img src="images/selection-strategy.png" alt="Choosing a selection strategy" width="600">
</p>

## Compatibility and limitations

- Minecraft Bedrock 1.26.30 and newer
- Both packs must be active; no other dependencies
- Standard graphics and Vibrant Visuals/PBR
- Single-player, multiplayer, Realms, and compatible Bedrock servers
- All dimensions. Survival and Adventure; Creative works, Spectator is skipped
- No cheats, commands, experimental toggles, or required dependencies
- Blocks from other add-ons that the engine does not recognise are left alone rather than guessed at
- **Do not run two automatic tool switchers in one world** — both will fight for the selected slot
- Whole-inventory search restores your layout, but deliberately skips the restore if you rearrange your inventory mid-swing, which can leave a borrowed tool in place. Hotbar-only search never moves anything

See [Compatibility and Troubleshooting](https://github.com/CharlesJGantt/Andys-Smart-Tool-Swapper/wiki/Compatibility-and-Troubleshooting) for detailed diagnostics.

## Support AndyTheMakerMC

All of my Minecraft Bedrock add-ons are free to download and use. If one of my add-ons has improved your world, saved you time, or added something you wish Minecraft already had, consider supporting continued development. Your support helps fund the time and tools required to maintain existing add-ons, test new Minecraft Bedrock releases, fix bugs, create documentation and artwork, and continue building new add-ons.

**Help me keep these add-ons free, updated, and actively maintained** — support through [Buy Me a Coffee](https://www.buymeacoffee.com/AndyTheMakerMC) or a direct donation through [Stripe](https://buy.stripe.com/4gM4gz0qu0xwgxw0IfcMM00). Prefer another way? [Ko-fi](https://ko-fi.com/andythemaker) · [Patreon](https://www.patreon.com/cw/AndyTheMakerMC) · [GitHub Sponsors](https://github.com/sponsors/CharlesJGantt). Every bit of support is appreciated, but it is never required.

Enjoying the add-on? Ratings, favorites, recommendations, and kind comments also help more Bedrock players discover Andy's work.

### Explore more of Andy's add-ons

Visit [AndyTheMakerMC.xyz](https://andythemakermc.xyz/) for more Minecraft Bedrock add-ons, `.mcstructure` downloads, HoloPrint files, world lore, tutorials, guides, videos, and other creations.

### Follow AndyTheMakerMC

Follow **@AndyTheMakerMC** for new add-on releases, development updates, tutorials, showcases, streams, and more Minecraft adventures, and join the community on Discord and Facebook:

- [YouTube](https://www.youtube.com/@AndyTheMakerMC)
- [Twitch](https://www.twitch.tv/AndyTheMakerMC)
- [TikTok](https://www.tiktok.com/@AndyTheMakerMC)
- [Instagram](https://www.instagram.com/andythemakermc/)
- [X (Twitter)](https://x.com/AndyTheMakerMC)
- [Discord](https://discord.gg/KVFNHf67Y)
- [Facebook Group](https://www.facebook.com/groups/1728623358327048)

## End-user permission

You may download the official, unmodified release of Andy's Smart Tool Swapper from its official CurseForge or authorized GitHub project page and install, activate, and use it in personal single-player worlds, multiplayer worlds, Realms, and compatible Bedrock servers.

This permission includes Minecraft's normal automatic delivery of the official, unmodified add-on to players joining a world, Realm, or server where it is active. It does not permit offering the add-on file separately or distributing it as part of a world download, modpack, bundle, mirror, archive, or server download.

## Content-creator permission

Content creators may use an official, unmodified release of Andy's Smart Tool Swapper in original gameplay videos, livestreams, screenshots, tutorials, reviews, showcases, articles, guides, social posts, and other original content, including monetized content.

Credit to **AndyTheMakerMC** and a link to the official CurseForge project page are appreciated whenever practical. This permission covers display of normal gameplay and commentary; it does not grant permission to redistribute, modify, extract, or republish the add-on or its assets.

## License — All Rights Reserved

**All Rights Reserved. Copyright © 2026 Andy / AndyTheMakerMC.**

You may not redistribute, reupload, rehost, mirror, resell, sublicense, bundle, repackage, modify and publish, translate, adapt, decompile, disassemble, reverse engineer, extract, or reuse the add-on, its source code, scripts, documentation, branding, textures, models, pack icons, or promotional artwork without prior written permission from the copyright holder.

You may not create derivative works or incorporate any portion of the project into another add-on, Behavior Pack, Resource Pack, application, product, modpack, download, or project without prior written permission. The end-user and content-creator permissions above are limited permissions; they do not transfer ownership or grant redistribution rights.

The promotional artwork is original AI-assisted concept artwork directed for this project. It is not an in-game screenshot.

Minecraft is a trademark of Microsoft Corporation. This project is not affiliated with, endorsed by, sponsored by, or associated with Microsoft or Mojang Studios.
