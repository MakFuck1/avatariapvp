# Avataria  PVP
Avataria PVP, kendi avataria sunucunuzu kurmanızı sağlar.

# VDS - VPS Üzerine Kurulum
- apt-get update
- apt-get upgrade
- apt install python3-pip
- apt-get install redis-server
- systemctl enable redis-server.service
- git clone https://github.com/emirkibar/avatariapvp-tr
- "avatariapvp-tr" dosyasının içindeki "web.ini" yi kendi sunucunuza göre güncelleyin.
- pip3 install --user -r requirements.txt  oyun gereksimilerini indirin.
- Uzak Masaüstü Bağlantısından makinanızda terminal açıp "cd avatariapvp-tr" yazıp python3 web.py yazın.
- Yeni bir terminal açıp yine cd avatariapvp-tr yazıp python3 server yazıp sunucuyu başlatın.

# XRDP Kurulumu (Uzak Masaüstü Erişimi Sağlar)
- sudo apt update
- sudo apt install xfce4 xfce4-goodies xorg dbus-x11 x11-xserver-utils
- sudo apt install xrdp 
- sudo systemctl status xrdp
- xrdp.service - xrdp daemon
   Loaded: loaded (/lib/systemd/system/xrdp.service; enabled; vendor preset: enabled)
   Active: active (running) since Sun 2019-07-28 22:40:53 UTC; 4min 21s ago
     Docs: man:xrdp(8)
           man:xrdp.ini(5)
- sudo adduser xrdp ssl-cert  
- sudo systemctl restart xrdp


