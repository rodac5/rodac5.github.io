# Linux
## Montar smb
sudo mount -t cifs -o ro,vers=3.0,credentials=/root/.smbcredentials //<ip>/<share/ /mnt/<mountpoint>
> /root/.smbcredentials:
username=<user>
password=<password>
domain=<domain>

