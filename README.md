# Atlanta Server modpack

Mods and setup for the Atlanta Minecraft server (Java Edition 26.3, Fabric).
You need these mods to join. The server rejects a plain Minecraft client.

To get the server address, contact the server admin, Kurt.

## Quick setup (about 3 minutes)

1. Install [Prism Launcher](https://prismlauncher.org/download/).
2. Download [Atlanta-Server-Instance.zip](https://github.com/thefluxster/atlanta-pack/raw/main/Atlanta-Server-Instance.zip). Do not unzip it.
3. In Prism, choose **Add Instance**, then **Import from zip**, and select the file.
4. Press **Play**. The first launch downloads the mods and takes a few minutes. Prism asks to install Java 25 if you don't have it. Say yes.
5. In Minecraft, go to **Multiplayer**, then **Add Server**, and enter the server address you got from Kurt.

Every time you press Play, the launcher checks this page for changes and updates your mods to match the server. Do not add or remove mods by hand in this instance. Make a separate instance for your own mods.

## New players: read this first

### Server rules
- **No griefing and no stealing.** Either one gets you banned. This includes looting someone else's grave.
- **PvP only by agreement.** PvP is technically on, so ask first. Attacking someone who hasn't agreed counts as griefing.
- **Difficulty is Hard.** Mobs hit hard, hunger can kill you, and the RPG mobs are tuned for groups. Expect to die early on.

### When you die
A **grave** appears where you died and holds all your items and XP. Only you can open it, and it never expires. Go back and right-click it. If you died somewhere awful, the grave's menu tells you where it is.

### The world
- The terrain is reworked: huge continents, new biomes, and a remade Nether and End. Most things look different from vanilla.
- There are many new structures: dungeons, taverns, ocean ruins and towers. **Shrine Towers** have a trial at the top whose reward is a **Shrine Chart**, a map to a Shrine. Shrines run from Tier I to Tier VI. Tier VI is brutal, so bring a group.
- Many new animals and monsters. Watch out for **Mutant** zombies, skeletons, creepers and endermen. They're mini-bosses: don't fight one alone.
- Pre-generated land near spawn loads fast. Far-out unexplored land is slower, and the server may briefly stop you at the edge while it builds the terrain. This is normal.

### The RPG side (optional, but it's how you get strong)
1. **Pick a path.** There are nine: Arcane, Fire or Frost Wizard, Paladin, Priest (the healer), Rogue, Warrior, and Archer. Your path is set by your **spell book**, which you equip in its own slot.
2. **Get spells.** Craft a **Spell Binding Table** (a book over amethyst, a gold ingot and amethyst, on polished diorite) and use it to make your class book and bind spells to it. This costs XP levels and lapis.
3. **Cast.** Hold a class weapon (a staff, wand, bow, dagger and so on). Your spells appear on a **spell hotbar**. Set the keys under **Options → Controls → Spell Engine**.
4. **Fuel.** Wizards and Paladins/Priests use up **runes** when they cast. Craft runes by hand, or at a **Rune Crafting Altar**, which is cheaper. A **Rune Pouch** holds them.
5. **Level up your skills.** Killing mobs earns **skill points**, and tougher mobs earn more. Points are shared with teammates within 200 blocks, so grouping up levels everyone. Open the skill tree with the key the game names when you earn your first point (it's also under **Controls → Skills**). There are two trees: **Class Skills**, which are locked to one class (up to 13 points), and **Weapon Skills** (up to 6). An **Orb of Oblivion** resets your class skills (a diamond surrounded by bottles o' enchanting).
6. **Gear up.**
   - **Jewelry:** rings and necklaces from Jeweler villagers and gems.
   - **Relics:** trinkets with active abilities.
   - **Armory:** class armor sets. Upgrade them to epic tiers with crystals at a smithing table.
   - **Arsenal:** legendary weapons. Win these from bosses and dungeons; you can't craft them.

**How to succeed:** play as a group of mixed classes, the way you would in Minecraft Dungeons. A Warrior or Paladin holds the mob's attention, a Priest heals, and Wizards, Rogues and Archers deal the damage. Roll out of attacks (**Combat Roll**, key under Controls). Swing with rhythm rather than spam-clicking: weapons have combos. Don't go after Mutants or high-tier Shrines without a healer.

## Setup without the zip

Use this if the import fails.

1. Install Prism Launcher and create a new instance: Minecraft **26.3**, Fabric loader **0.19.5**.
2. Download [packwiz-installer-bootstrap.jar](https://github.com/packwiz/packwiz-installer-bootstrap/releases/latest). In Prism, open **Instance > Folders > Minecraft** and put the file in that folder.
3. Open **Instance > Settings > Custom commands**, tick **Custom commands**, and set the pre-launch command to:
   ```
   "$INST_JAVA" -jar packwiz-installer-bootstrap.jar https://raw.githubusercontent.com/thefluxster/atlanta-pack/main/pack.toml
   ```
4. Press Play, then add the server as in step 5 above.

## Voice chat

Simple Voice Chat is included and works by distance: people hear you when you are close.
Press **V** in game to open the voice chat menu and set up your microphone.

## Memory

If the game is slow or crashes while loading, give it more memory in Prism under **Settings > Java > Maximum memory allocation**. 4096 MB is a reasonable minimum, and 6144 MB is better if your computer has 16 GB or more.

## Troubleshooting

- **"Mismatched mod" or registry error when joining.** Your mods are out of date. Close the game, press Play again from Prism and wait for the update to finish, then retry.
- **Prism reports the pre-launch command failed.** Check your internet connection and try again. If it keeps failing, contact the server admin, Kurt.
- **Can't connect at all.** Check the address with Kurt. The server may also be restarting. It stops nightly around 02:50 and is back by about 03:10 (US Pacific time).

## What is in the pack

Mods that run on the server and on your computer:

- Simple Voice Chat
- Better Archeology
- Farmer's Delight (Refabricated)
- Naturalist
- Alex's Mobs Continued (mobs Naturalist already has are turned off)
- Mutant Monsters
- Sea Life
- Combat Roll
- Better Combat
- RPG Series: Wizards, Archers, Paladins & Priests, Rogues & Warriors, Jewelry, Relics, Armory, Arsenal, Skill Tree (with Pufferfish's Skills and Critical Strike)
- FerriteCore (memory savings)
- Libraries these depend on (Fabric API, Cloth Config, Spell Engine and others)

Mods that only run on your computer (installed automatically, optional for gameplay):

- Sodium, Entity Culling, ImmediatelyFast, Dynamic FPS (performance)
- LambDynamicLights (held torches and glowing items light up the area around you)
- Xaero's Minimap and Xaero's World Map
- Sound Physics Remastered

Mods that only run on the server (you don't download these):

- William Wythers' Overhauled Overworld, Continents, Incendium, Nullscape
- Dungeons and Taverns, Moog's Ocean Structures, Gazebos
- Axes Are Weapons
- Universal Graves (owner-only graves, no time limit)
- Lithium, Krypton, ServerCore, Chunky (server performance)

## For the server admin

Pack source files are `pack.toml`, `index.toml`, the `mods/` folder and `config/` (shipped mod settings: `amc.json` Alex's Mobs spawns, `servercore/config.yml` dynamic distances under load, `universal-graves/config.json` permanent owner-only graves), managed with [packwiz](https://packwiz.infra.link/).
After changing mods, run `packwiz refresh`, commit and push. The server syncs from its local copy on every start. Clients sync from this repository's raw files on every launch, and GitHub can take up to five minutes to serve new versions.
