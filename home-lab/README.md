# Home Lab

Started **September 2026**. Built mostly from secondhand and free equipment to practice Linux administration, networking, and security hands-on.

## Hardware
| Device | Role |
|---|---|
| ASUS L410M laptop | Server running Ubuntu Server 24.04 LTS |
| TP-Link TL-SG705 (5-port, unmanaged) | Main switch |
| TP-Link TL-SG1005D (5-port gigabit) | Extra switch |
| Netgear GS608 v2 (8-port gigabit) | Extra switch |
| ARRIS SURFboard SB6141 | Cable modem |
| Cat6 UTP solid 23AWG cables | Cabling |

## Network diagram
<!-- TODO: add a simple diagram (draw.io, Excalidraw, or a photo of a sketch) -->
![Home lab diagram](screenshots/diagram.png)

## Services
| Service | How it runs | Purpose |
|---|---|---|
| Pi-hole | Docker container | Network-wide DNS filtering and ad blocking |
| File share | <!-- TODO: Samba? NFS? --> | Central storage for devices on the network |
| SSH | systemd | Remote admin, hardened (see below) |

## SSH hardening
What I changed in `/etc/ssh/sshd_config` and why:
<!-- TODO: fill in only what you actually did. Common examples: -->
- [ ] Key-based login only (`PasswordAuthentication no`). Why:
- [ ] Root login disabled (`PermitRootLogin no`). Why:
- [ ] Changed port / limited users (`AllowUsers`). Why:
- [ ] fail2ban or UFW firewall rules. Why:

How I verified it worked:
```
# TODO: paste a test, e.g. trying a password login and showing it was refused
```

## Docker setup
Configs live in [`configs/`](configs/). **Remove passwords and the Pi-hole web password before committing.**

## Problems I hit and how I fixed them
| Problem | Cause | Fix |
|---|---|---|
| <!-- TODO --> | | |

## Next
- VLAN segmentation (needs a managed switch)
- Dedicated firewall: pfSense or OPNsense
- Centralized logging / SIEM practice (e.g. Wazuh)
