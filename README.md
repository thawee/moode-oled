# moode-oled
display Moode welcome screen, and playing song info, inspired by mpd_oled and moode-old 
 - welcome screen
 - display music title and resolutions
 - support every language (unicode-8)

# Hardware
oled sh1106 i2s board connecting to PI as xxxx

# Software
developed in python3 using luma library to display on oled screen  

# HLD
utilising Moode lcd updater concept, the screp will read currentsong.txt on /var/local/www/currentsong.txt and display on oled screen

# installation
install luma dependency
install mode-oled
/var/local/www/commandw/lcd_updater.py
/var/local/www/commandw/fonts/*.ttf

# run on startup
/etc/rc.d/rc.local

# moode configuration
enable song metadata
enable lcd updater
