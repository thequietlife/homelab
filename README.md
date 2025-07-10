# Notes


Aim: Securing my home office network. ‘Raising the bar’. ‘purpose built devices rather than all in one’: Joff Thyer. 

Hardware:

- 2 x Lenovo ThinkCentre M910q $199 x 2
- GL.iNet Slate AX (GL-AXT1800) $110
- Netgear 8 port managed switch $91
- CAT 6 Ultra Thin Ethernet Cables $12
- Total: $610.64

Software:
- mullvad VPN $9/month

Process:
- ASUS RT-AX86S router: using guest network for homelab
- GL-AXT1800 set up (repeater)
- Mullvad VPN for GL-AXT1800
- Netgear GS108E switch. (802.1Q) Use Netgear Discovery Tool to access admin panel. GL-AXT1800 plugged into port 1
- If switch does not connect. Press factory defaults. Will then need add new password
- Switch firmware update: select .bin file not whole zip folder
- GL-AXT1800 has two VLANS out of the box: Private and Guest
- Updated passwords wifi
- VLANs: Virtual ports on top of physical ports. Connect devices to separate networks - Guest network, smart devices, video surveillance devices
- LuCI












__________________
Sources: 
1. [Pandemic Paradigm Shift - Remote working is the New Normal, Black Hills Information Security](https://www.youtube.com/watch?v=Oon_SGqxu4g&t=2733s)
2. [Home Router Setup | OPNSense, The Smoking Cap](https://www.youtube.com/watch?v=Kah0OTKieEU)


