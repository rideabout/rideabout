## Proxmox Notes

### Copying iso files to proxmox server

If issues occur copying iso files to the proxmox server via the web interface, here are some additional options to copy iso files to the iso directory of the proxmox server for various OSes.

#### Linux

Russ~/Downloads$ scp -v ubuntu-12.04-beta1-dvd-amd64.iso root@192.168.0.137:/var/lib/vz/template/iso

This transferred my Ubuntu-12.04 Beta iso (which I downloaded from the Ubuntu Web Page to /home/russ/Downloads) to my Proxmox VE server's /var/lib/vz/template/iso directory. The Proxmox VE server is located on my local LAN at ip 192.168.0.137.

#### Windows

On Windows use the FileZilla SFTP client and root user account and password.