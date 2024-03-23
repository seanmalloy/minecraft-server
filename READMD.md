# Minecraft Server (Java Edition)

Run a Minecraft server in a container on Fedora Server.
```
sudo firewall-cmd --zone=FedoraServer --add-port=25565/tcp --permanent
sudo firewall-cmd --reload
podman run -it -d --name minecraft -p 25565:25565 -e EULA=TRUE -e VERSION=1.20.4 -v /home/$USER/minecraft-data:/data:Z docker.io/itzg/minecraft-server:latest
```

# References
- [itzg/minecraft-server](https://hub.docker.com/r/itzg/minecraft-server)

