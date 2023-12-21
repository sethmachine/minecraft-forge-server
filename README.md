# minecraft-forge-server

This repo provides configuration for a private at home Minecraft Forge server.  

This server uses the docker image provided here: https://docker-minecraft-server.readthedocs.io/en/latest/types-and-platforms/server-types/forge/

## Run Server

Execute `docker compose up -d` in the same directory as the `docker-compose.yml`. 

## Gotchas

Server should only include server side mods.  Mods that are client side only will cause the server to fail to load, as they expected GUI libraries to exist.  