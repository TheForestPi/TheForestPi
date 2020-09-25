# The ForestPi Project

### setup raspberry pi
```
sudo raspi-config
```

- 4 Localisation Options => Timezone => Asia/Bangkok
- 5 Interfacing Options => I2C => Yes

### install rtc ds1307 module and add dtoverlay to config.txt
```
sudo nano /boot/config.txt
```

dtoverlay=i2c-rtc,ds1307

### install command
```
sudo apt update && sudo apt -y install git && cd ~ && rm -rf theforestpi && git clone https://github.com/TheForestPi/theforestpi && cd theforestpi && make && cd ~
```

### edit configurations
```
nano /home/pi/theforestpi/config.json
```

### reboot
```
sudo reboot
```
