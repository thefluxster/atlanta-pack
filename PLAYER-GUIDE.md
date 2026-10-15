# Joining the server (Minecraft 26.3, Fabric)

1. Install Prism Launcher (prismlauncher.org).
2. Create a new instance: Minecraft 26.3, Fabric loader 0.19.5.
3. Download packwiz-installer-bootstrap.jar from
   https://github.com/packwiz/packwiz-installer-bootstrap/releases/latest
   and put it in the instance's Minecraft folder (Instance > Folders > Minecraft).
4. Open the instance, then Settings > Custom commands.
   Tick "Custom commands" and set Pre-launch command to:
   "$INST_JAVA" -jar packwiz-installer-bootstrap.jar https://raw.githubusercontent.com/thefluxster/atlanta-pack/main/pack.toml
5. Launch. Every launch syncs your mods with the server. Do not add or remove mods by hand.
6. Multiplayer > Add Server > keyserhome.ddns.net

Voice chat: press V to set up your microphone the first time.
