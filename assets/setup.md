### 🚧 Setting up my lab

My homelab journey started with virtual machines (VMs) loaded onto an external hard drive (SanDisk Extreme Portable SSD 1TB). Here I was able to have a play with Kali and a few different versions of Windows.

<p align="center">
<img
src="https://github.com/thequietlife/malware-analysis/blob/d2fb83843cf68c1bf3261e292822cc7ce886191d/images/iMac.jpeg"
alt="2017 iMac with ubuntu as the operating system" width="400"/>
</p>
I moved onto a 2017 iMac that had been gifted to me by a family member. I have a neat Apple A1048 keyboard I found from a business that was moving. I set up Ubuntu on the iMac. This involved using balenaEtcher to create a bootable USB drive. It's pretty cool to bring a 2017 iMac back to life with a fresh operating system. For my hypervisor I have opted for Oracle VirtualBox. 


My current set up is a mini lab. I had a clear idea of what I wanted it to look like and what I wanted to achieve - a physically small setup, a space for my lab which was separate from the other devices in the house with VLANs. VLANs are virtual ports that sit on top of the switch’s physical ports. They let you connect devices to separate networks. I used draw.io to mock it up and asked for feedback in the pilar discord group. I got great feedback on how to set up a temporary, low cost lab. Using a travel router to piggy back on my existing ASUS router. I bought a Netgear GS108E 8 port managed switch, two tiny Lenovo M910q desktop PCs and a few CAT 6 ethernet cables.

Building a homelab stayed on my To Do list for quite a while. It was a bit daunting to get started. Some of the homelabs on reddit.com/r/homelab are huge. A buddy pointed me toward [Serve The Home's Project TinyMiniMicro Home Lab Revolution](https://www.servethehome.com/introducing-project-tinyminimicro-home-lab-revolution/). I also found reddit.com/r/minilab/ which was useful to see what others had made. I had to stop scrolling and start. Knowing what to start with was tricky. How do I use a switch to get VLANs set up? I started with setting up the GL.iNet Slate AX 1800 travel router. I use the repeater method. I also set up VPN through the travel router’s admin panel. Next was the switch. It wasn’t all that scary setting up VLANs. A few YouTube videos, reading and re-reading the Netgear documentation. I configured VLANs on the switch and via LuCl, OpenWrt for the router. Now I have two separate networks to use for my tech playground.

The mini lab took about one week to set up. I was determined to get it set up and not get too distracted or despondent when things didn’t come together the first time. It was on my To Do list for too long and needed to just get done. It’s been great to ‘raise the bar’ of my home network. But also get a win to build my confidence with doing something pretty technical.
__________________
Sources: 
- [Joff Thyer, [Pandemic Paradigm Shift Remote working *is* the New Normal](https://www.blackhillsinfosec.com/wp-content/uploads/2020/09/SLIDES_PandemicParadigmShift.pdf)

- [Kyle Cucci's Evasive Malware: Understanding Deceptive and Self-Defending Threats](https://nostarch.com/evasive-malware). 

- [Michael Sikorski and Andrew Honig's Practical Malware Analysis](https://www.amazon.com/Practical-Malware-Analysis-Hands-Dissecting/dp/1593272901). 
