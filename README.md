# Atlanta Server modpack

Mods and setup for the Atlanta Minecraft server (Java Edition 26.3, Fabric).
You need these mods to join. The server rejects a plain Minecraft client.

Server address: `keyserhome.ddns.net`

## Quick setup (about 3 minutes)

1. Install [Prism Launcher](https://prismlauncher.org/download/).
2. Download [Atlanta-Server-Instance.zip](https://github.com/thefluxster/atlanta-pack/raw/main/Atlanta-Server-Instance.zip). Do not unzip it.
3. In Prism, choose **Add Instance**, then **Import from zip**, and select the file.
4. Press **Play**. The first launch downloads the mods and takes a few minutes. Prism asks to install Java 25 if you don't have it. Say yes.
5. In Minecraft, go to **Multiplayer**, then **Add Server**, and enter `keyserhome.ddns.net`.

Every time you press Play, the launcher checks this page for changes and updates your mods to match the server. Do not add or remove mods by hand in this instance. Make a separate instance for your own mods.

## Setup without the zip

Use this if the import fails.

1. Install Prism Launcher and create a new instance: Minecraft **26.3**, Fabric loader **0.19.5**.
2. Download [packwiz-installer-bootstrap.jar](https://github.com/packwiz/packwiz-installer-bootstrap/releases/latest). In Prism, open **Instance > Folders > Minecraft** and put the file in that folder.
3. Open **Instance > Settings > Custom commands**, tick **Custom commands**, and set the pre-launch command to:
   ```
   "$INST_JAVA" -jar packwiz-installer-bootstrap.jar https://raw.githubusercontent.com/thefluxster/atlanta-pack/main/pack.toml
   ```
4. Press Play, then add the server address as above.

## Voice chat

Simple Voice Chat is included and works by distance: people hear you when you are close.
Press **V** in game to open the voice chat menu and set up your microphone.

## Memory

If the game is slow or crashes while loading, give it more memory in Prism under **Settings > Java > Maximum memory allocation**. 4096 MB is a reasonable minimum, and 6144 MB is better if your computer has 16 GB or more.

## Troubleshooting

- **"Mismatched mod" or registry error when joining.** Your mods are out of date. Close the game, press Play again from Prism and wait for the update to finish, then retry.
- **Prism reports the pre-launch command failed.** Check your internet connection and try again. If it keeps failing, tell the server admin.
- **Can't connect at all.** The server may be restarting. It stops nightly around 02:50 and is back by about 03:10 (US Pacific time).

## What is in the pack

Mods that run on the server and on your computer:

- Simple Voice Chat
- Better Archeology
- Farmer's Delight (Refabricated)
- Naturalist
- Sea Life
- Combat Roll
- Better Combat
- RPG Series: Wizards, Archers, Paladins & Priests, Rogues & Warriors, Jewelry
- Libraries these depend on (Fabric API, Cloth Config, Spell Engine and others)

Mods that only run on your computer (installed automatically, optional for gameplay):

- Sodium (performance)
- Xaero's Minimap and Xaero's World Map
- Sound Physics Remastered

Mods that only run on the server (you don't download these):

- William Wythers' Overhauled Overworld, Continents, Incendium, Nullscape
- Dungeons and Taverns, Moog's Ocean Structures, Gazebos

## For the server admin

Pack source files are `pack.toml`, `index.toml` and the `mods/` folder, managed with [packwiz](https://packwiz.infra.link/).
After changing mods, run `packwiz refresh`, commit and push. The server syncs from its local copy on every start. Clients sync from this repository's raw files on every launch, and GitHub can take up to five minutes to serve new versions.
