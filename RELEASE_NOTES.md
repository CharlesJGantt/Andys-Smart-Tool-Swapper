# Andy's Smart Tool Swapper 0.2.3

Initial release. Automatic tool switching that picks the right tool **and** the right enchantment for the block you are breaking, then hands your previous item straight back.

## What it does

- **Automatic tool selection** for pickaxes, axes, shovels, hoes, shears and melee weapons, covering the blocks other switchers miss — sculk, sponge, hay, bamboo, muddy mangrove roots, nether stems, copper in every state, cobwebs, wool, leaves and chains. Decorated pots and flower pots correctly ask for no tool at all.
- **Fortune and Silk Touch are treated as choices about the drop.** By default a tool you deliberately picked up is never swapped away. Smart mode instead picks the enchantment each block deserves — Fortune on ores and gravel, Silk Touch on glass, ice, sculk, grass blocks and spawners.
- **Return to your previous item.** Hold a torch, break stone, get the torch back. The add-on borrows; it does not take over.
- **It follows what you do, not where you look.** A swap begins when you start breaking something, not when your crosshair drifts past a chest. Once you have started, the tool keeps up as the material changes — stone, gravel, dirt, log, stone — without you releasing the button.
- **Four selection strategies:** Balanced, Fastest, Preserve Valuable Gear and Lowest Adequate Tier. Efficiency is read with the real formula, so an Efficiency V iron pickaxe genuinely outranks a bare Netherite one under Fastest.
- **Three durability policies**, plus a safety floor that refuses tools close to breaking so nothing you are handed dies mid-swing.
- **Area-mining tools are never auto-selected** unless you switch them on. A 3×3 Hammer equipped to fix one misplaced block would take eight of its neighbours with it.
- **Mark any individual tool** Preferred or Never auto-select. The mark follows that exact item, so one of two identical Netherite pickaxes can be off limits while the other stays in the rotation.
- **Teach Smart Tool Swapper** registers custom tools from other add-ons that declare nothing readable, so third-party gear works without either creator shipping a patch.
- **Hold sneak to pause it** entirely — no menu, no command. Builder protection keeps it out of your way while placing blocks, and Combat Lock stops a pickaxe appearing mid-fight.
- **Why did it pick that tool?** reads back every candidate it considered, in score order, with the reason each one won or lost.

## Configuring it

The add-on adds **no items and no blocks**. Both menus open from a plain stick renamed on an anvil, matched exactly including capital letters:

- **`SwapperControl`** — your own settings. Anyone can make one.
- **`AdminSwapperControl`** — the world settings and Teach Smart Tool Swapper. Operators only.

Every setting has a per-player version, and the world owner decides whether players may change their own. World defaults can also be set from the gear icon beside the pack at world creation.

## Multiplayer and dedicated servers

Works on Realms, LAN and dedicated servers, with per-player settings. Dedicated servers configure everything from the console — `/scriptevent andy_sts:help` lists all sixteen commands. Console commands are authorized by the event source, so the server console is never refused for the lack of a player behind it.

## Compatibility

- Requires Minecraft Bedrock **1.26.30 or newer**.
- **No experiments, no beta APIs, no cheats.** Stable Script API only.
- **Achievement friendly** — verified in game on a clean world.
- Renders correctly on Standard graphics and under **Vibrant Visuals**.
- Includes linked Behavior and Resource Packs; activating either one activates the other.
- No dependencies.

Optional companions, none required: **Andy's Advanced Durability Guard** (a tool inside the Guard's reserve is never selected), **Andy's Advanced Hammers, Excavators & More** (recognised as area tools and held back by default), **Andy's Silk Touch Relics** (spawners, vaults, budding amethyst and end portal frames ask for Silk Touch), and **Andy's Configurable Vein Miner & Tree Capacitor** (the swap lands before the block breaks).

Do not run two automatic tool switchers in one world — both will fight for the selected slot.

## Full player guide

Every setting, every menu and the complete console reference:
**https://github.com/CharlesJGantt/Andys-Smart-Tool-Swapper/wiki**

---

*Version numbering starts above 0.1.0 because the add-on went through several internal builds and play-test rounds before this first public release. Nothing before 0.2.3 was published.*
