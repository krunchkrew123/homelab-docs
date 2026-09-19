# Proxmox VE Home lab server

## Purpose
The purpose of building out this lab is to gain hands on sysadmin, cybersecurity, and programming skills.

## Hardware
- Thinkstation P330, 32 gb RAM
- Storage : total: 1tb nvme SSD + 512 gb HDD

## Proxmox VE Install
- Version installed 9.2.4
- Install method: USB
- Had to remove the gpu to be able to use the hdmi adapter to view the display on my tv for install, installed 32gb of RAM was previously 8gb. Installed 1tb nvme ssd stick into the case was previously 512gb HDD.

## Network config
- Host net interfaces: WAN(vmbr0), vmbr1(opnsense LAN)
- IP scheme, ISP router- on vmbr0 192.168.x.x to opnsense- WAN(vmbr0) LAN(vmbr1) 10.10.x.x

## VMs Hosted
| Name | type (VM/LXC) | Purpose |
|---|---|---|
| Wazuh Manager | VM | SIEM |
| DevServer | VM | Development server to host services |
| OpnRoute | VM | Router/Firewall |
| Windows-server | VM | Practice AD Concepts |