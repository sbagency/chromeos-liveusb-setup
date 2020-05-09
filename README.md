# crome os usb setup

```bash
wget https://dl.bintray.com/chromebrew/chromebrew/parted-3.2-chromeos-x86_64.tar.xz
wget https://dl.bintray.com/chromebrew/chromebrew/ncurses-6.2-chromeos-x86_64.tar.xz
tar xvf ncurses-6.2-chromeos-x86_64.tar.xz
tar xvf parted-3.2-chromeos-x86_64.tar.xz
export LD_LIBRARY_PATH=/usr/local/opt/usr/local/lib64:$LD_LIBRARY_PATH
cd usr/local/sbin

sudo ./parted
print free
resizepart 16
quit

resize2fs /dev/sda16 
```
