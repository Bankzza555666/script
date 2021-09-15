สคริป​ OVPN+V2RAY

อย่าลืมเตรียมโดเมนก่อนนะครับ

<h3 align="center">ก่อนอื่นใส่คำสั่งนี้ก่อน</h3>

<p align="center">
<pre align="center">apt update && apt upgrade -y && update-grub && sleep 2 && reboot
</pre></p>

<h3 align="center">หลังเครื่องรีบูตแล้วใส่คำสั่งนี้ต่อ 
</h3>
<p align="center">
<pre align="center">sysctl -w net.ipv6.conf.all.disable_ipv6=1 && sysctl -w net.ipv6.conf.default.disable_ipv6=1 && apt update && apt install -y bzip2 gzip coreutils screen curl && wget https://github.com/wehoi/ws/raw/main/setup.sh && chmod +x setup.sh && screen -S setup.sh ./setup.sh
</pre></p>

ข้อมูลสคริป
- OpenSSH                 : 22
- OpenVPN                 : TCP 1194, UDP 2200, SSL 442
- Stunnel4                : 444, 777
- Dropbear                : 109, 143"  
- Squid Proxy             : 3128, 8080 (limit to IP Server)
- Badvpn                  : 7100, 7200, 7300
- Nginx                   : 81
- V2RAY Vmess TLS         : 8443
- V2RAY Vmess None TLS    : 80
- V2RAY Vless TLS         : 2083
- V2RAY Vless None TLS    : 8880
- Trojan                  : 2443
- Owner                   : SP VPN-TH
- LINE                    : BANKISSS


ซัพพอร์ต​

Debian 9 & 10
Ubuntu 18 & 20
