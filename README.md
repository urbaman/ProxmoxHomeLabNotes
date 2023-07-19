# ProxmoxHomeLabNotes
## Appunti vari sul progetto Proxmox
Il progetto Proxmox prevede di impostare un cluster di almeno tre nodi Proxmox, per far girare le seguenti istanze:

Plesk (mailserver)
- [ ] How to manage the mailserver with cloudflare

Proxmox (Hypervisor)
- [x] PfSense in HA
- [x] HomeAssistant (domotica)
- [x] 3x TrueNAS SCALE cluster (filesystem) - NOT WORKING
- [x] Truecommand to manage TrueNAS SCALE gluster cluster - NOT WORKING
- [x] Gluseterfs cluster
- [x] 3x haproxy for HA implementations
- [x] 3x etcd cluster for kubernetes
- [x] 3x ccontrol planes, 3x worker nodes kubernetes cluster
    - [x] Metallb Loadbalancer
    - [x] Multus multinetwork
    - [x] Longhorn storage
    - [x] Portainer
    - [x] Certmanager
    - [x] Traefik
    - [x] Proxmox monitoring (Prometheus-Grafana)
    - [x] Proxmox Backup monitoring (Prometheus-Grafana)
    - [x] Haproxy monitoring
    - [x] Dell Idrac Monitoring
    - [x] Arista switch monitoring
    - [x] Uptimekuma
    - [x] Kured
    - [x] Heimdall
    - [x] Datree
    - [x] Teleport (still not behind Traefik)
    - [ ] MySQL (MariaDB) and MySQL Prometheus-Grafana monitoring
    - [ ] Redis and Redis Prometheus-Grafana monitoring
    - [ ] NextCloud (FileServer) and Prometheus-Grafana monitoring
        - [ ] Nextcloud apps https://www.ionos.com/digitalguide/server/tools/nextcloud-apps/
        - [ ] Other nextcloud apps https://www.tecmint.com/nextcloud-apps/amp/
    - [ ] Plex (MediaServer) https://www.debontonline.com/2021/01/part-14-deploy-plexserver-yaml-with.html
        - [ ] With Sonarr, Radarr, Transmission, Jackett https://greg.jeanmart.me/2020/04/13/self-host-your-media-center-on-kubernetes-wi/
    - [ ] Boing shared computing
    - [ ] Vaultwarden https://github.com/dani-garcia/vaultwarden/wiki/Kubernetes-deployment
    - [ ] Authelia? https://www.authelia.com/integration/kubernetes/introduction/
    - [ ] Guacamole? https://github.com/thomas-illiet/k8s-guacamole
    - [ ] UrBackup (Backup)

https://github.com/awesome-selfhosted/awesome-selfhosted

### Server specs:
- Disco(i) per OS (3x250GB - raidz)
- Disco(i) per VMs (3x1 tera - raidz)
- Disco(i) per TrueNas con HBA in IT mode (3x4 tera - raidz)

### Appunti per how-to da seguire:
- Flash H310: https://fohdeesha.com/docs/H310.html
- Generale: https://www.kreaweb.be/diy-home-server-introduction/
- GPU distribuita: https://drive.google.com/drive/folders/15hGRYQGB69pES2GyUR9Q2zHVvEAVHxDa https://3os.org/infrastructure/proxmox/gpu-passthrough/pgu-passthrough-to-vm/#linux-virtual-machine-gpu-passthrough-configuration
- Post-install: https://opensourcelibs.com/lib/xshok-proxmox, https://opensourcelibs.com/lib/proxmox-zfs-postinstall
- Risorse varie: https://opensourcelibs.com/lib/awesome-proxmox-ve
- Ceph: https://blog.miniserver.it/proxmox/come-fare-un-cluster-proxmox-con-ceph/
