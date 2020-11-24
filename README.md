# sysroot-relativelinks

## sysroot opencv python
cd /opt
sudo mkdir sysroot
export ip_rpi=192.168.1.200
# dong bo hoa 
rsync -avz pi@$(ip_rpi):/usr/lib/python2.7/ sysroot/
rsync -avz pi@$(ip_rpi):/usr/include sysroot/usr
rsync -avz pi@$(ip_rpi):/usr/lib sysroot/usr
rsync -avz pi@$(ip_rpi):/opt/vc sysroot/opt
