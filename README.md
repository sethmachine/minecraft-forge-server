# minecraft-forge-server

This repo provides configuration for a private at home Minecraft Forge server.

This server uses the docker image provided here: https://docker-minecraft-server.readthedocs.io/en/latest/types-and-platforms/server-types/forge/

## Run Server

Execute `docker compose up -d` in the same directory as the `docker-compose.yml`.

## Gotchas

Server should only include server side mods.  Mods that are client side only will cause the server to fail to load, as they expected GUI libraries to exist.

## Minecraft setup
1.  Download and install the official Minecraft Launcher for your OS: https://www.minecraft.net/en-us/download
2.  Use Forge minecraft version: `1.12.2-14.23.5.2847`
3.  Download this installer JAR: [Forge Installer v1.12.2-14.23.5.2847](https://adfoc.us/serve/sitelinks/?id=271228&url=https://maven.minecraftforge.net/net/minecraftforge/forge/1.12.2-14.23.5.2847/forge-1.12.2-14.23.5.2847-installer.jar)
4.  On command line simply run `java -jar forge-1.12.2-14.23.5.2847-installer.jar`
5. Open your mods folder and unzip the mods and all the jars to install them.  On macOS go to this folder:
   ```/Users/<your user name here>/Library/Application\ Support/minecraft/mods/```
6. In the Minecraft launcher add a new launcher using forge.  