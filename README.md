<h1 align="center">
    Raspberry Giggle
</h1>
<h4 align="center">
    Raspberry server docker softwares
</h3>
<p align="center">
    <img src="https://img.shields.io/github/last-commit/wesleyadriann/raspberry_giggle" />
    <img src="https://img.shields.io/github/license/wesleyadriann/raspberry_giggle" />
    <img src="https://img.shields.io/github/repo-size/wesleyadriann/raspberry_giggle" />
</p>


### Softwares

- [ArchiSteamFarm](https://github.com/JustArchiNET/ArchiSteamFarm) ✔️
- [Pi-hole](https://pi-hole.net) ✔️
- [Dozzle](https://dozzle.dev/) ✔️
- [Samba](https://www.samba.org) ⚠️

✔️ Done | ⚠️ Doing

### Docker Images

- [ArchiSteamFarm](https://hub.docker.com/r/justarchi/archisteamfarm)
- [Pi-hole](https://hub.docker.com/r/pihole/pihole)
- [Dozzle](https://hub.docker.com/r/amir20/dozzle/)
- [Samba](https://hub.docker.com/r/servercontainers/samba)


### Setting up (optional)

Docker - disable unnecessary software steps in docker-compose.yml  
ArchiSteamFarm - put the settings in ./archi_steam_farm_config ([setting up](https://github.com/JustArchiNET/ArchiSteamFarm/wiki/Setting-up))  
Samba - set user and local to share in enviorement variables ([setting up](https://github.com/ServerContainers/samba#environment-variables-and-defaults))  

### Running
```sh
docker-compose up --build &
```

### Additional information

#### Web interface

ArchiSteamFarm IPC: [http://localhost:3333](http://localhost:3333)  
Pi-hole admin: [http://localhost/admin](http://localhost/admin)  

#### Others

get Pi-hole admin password
```sh
docker logs pi_hole | grep random
```
