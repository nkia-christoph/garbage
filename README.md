sudo ln -s /home/garbage/garbage/klipper_config/printer.cfg /home/garbage/klipper/config/printer.cfg


https://docs.armbian.com/User-Guide_Fine-Tuning/#swap-for-experts
$ sudo dd if=/dev/zero of=/media/swap bs=64M count=8 
$ sudo mkswap /media/swap
$ sudo chmod 600 /media/swap 
$ sudo swapon /media/swap 
$ sudo nano /etc/fstab
/media/swap none swap defaults 0 0
$ swapon --show