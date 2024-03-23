# Minecraft Server (Java Edition)

```
podman run -d -p 25565:25565 -e EULA=TRUE -e VERSION=1.20.4 -v /home/$USER/minecraft-data:/data:Z docker.io/itzg/minecraft-server:latest
```

