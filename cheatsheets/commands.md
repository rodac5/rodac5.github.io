# Linux
## Montar smb
sudo mount -t cifs -o ro,vers=3.0,credentials=/root/.smbcredentials //<ip>/<share/ /mnt/<mountpoint>
> /root/.smbcredentials:
username=<user>
password=<password>
domain=<domain>

## Montar encase
ewfmount image.E01 ./rawimage
mount ./rawimage/ewf1 ./mountpoint -o ro,loop,show_sys_files,streams_interace=windows,offset=$((<part_beginning>*512)) 
