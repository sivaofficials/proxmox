# Proxmox

nas and other docker like including template
github tutorial:
```
https://github.com/CarmineCodes/Make-a-network-drive-on-linux
```
protrainer template:
```
https://github.com/novaspirit/pi-hosted
```
```
https://raw.githubusercontent.com/pi-hosted/pi-hosted/master/template/portainer-v2-amd64.json
```
docker:
```
curl -sSL https://get.docker.com/ | sh
```
portrainer
```
docker run -d -p 9000:9000 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce
```
remove unused disk space
```
lvremove /dev/pve/data
```

lvresize -l +100%FREE /dev/pve/root
```
```
resize2fs /dev/mapper/pve-root
```

add dns 8.8.8.8 to slove dns issue


