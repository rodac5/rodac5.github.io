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

## grep + mv
grep -irl malware |xargs mv -t ../d2/
  
## fix "inconsistent tab and spaces" error in vim:
  https://vi.stackexchange.com/questions/27219/fixing-tab-and-space-inconsistency/27220#27220?newreg=7ed5976f468c499ab626ec6cdb481859

set softtabstop=4\
set tabstop=4\
set shiftwidth=4\
set expandtab\
Then, use :retab to fix the indentation issue in your code.
