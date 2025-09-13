### 🚧 Setting up my homelab

My homelab journey started with virtual machines (VMs) loaded onto an external hard drive (SanDisk Extreme Portable SSD 1TB). Here I was able to have a play with Kali and a few different versions of Windows.

I moved onto a 2017 iMac that had been gifted to me by a family member. I have a neat Apple A1048 keyboard I found from a business that was moving. 

<p align="center">
<img
src="https://github.com/thequietlife/homelab/blob/d3def557ffc74405cc6a1d83393ed6a2bc0e1352/images/iMac.jpeg"
alt="2017 iMac with ubuntu as the operating system" width="600"/>

I set up Ubuntu on the iMac. This involved using balenaEtcher to create a bootable USB drive. It's pretty cool to bring a 2017 iMac back to life with a fresh operating system. For my hypervisor I have opted for Oracle VirtualBox. I like the VirtualBox UI and it's pretty easy to get the hang of.

<p align="center">
<img
src="https://github.com/thequietlife/homelab/blob/e7d33f696b2d1d03df5f271d80b34e5cadad777b/images/iMac_VM.png"
alt="iMac desktop showing Oracle VirtualBox" width="600"/>

**Mini Lab** <br>

My current set up is a mini lab. I had a clear idea of what I wanted to achieve - a physically small setup and for my lab to be separate from the other devices in the house by using VLANs. VLANs are virtual ports that sit on top of the switch’s physical ports. They let you connect devices to separate networks. 

<p align="center">
<img
src="https://github.com/thequietlife/homelab/blob/25f6a53df2c68b4242b6387b07729ab91a634a42/images/minilab.jpeg"
alt="desk with a small travel router on top of a switch and two Lenovo tiny PCs; retro apple keyboard" width="600"/>

I used draw.io to mock it up and asked for feedback in the pilar discord group. I got great feedback on how to set up a temporary, low cost lab. Using a travel router to piggy back on my existing ASUS router. I bought a Netgear GS108E 8 port managed switch, two tiny Lenovo M910q desktop PCs and a few CAT 6 ethernet cables.

Building a homelab stayed on my To Do list for quite a while. It was a bit daunting to get started. Some of the homelabs on [reddit.com/r/homelab](reddit.com/r/homelab) are 🏢 huge. A buddy pointed me toward [Serve The Home's Project TinyMiniMicro Home Lab Revolution](https://www.servethehome.com/introducing-project-tinyminimicro-home-lab-revolution/) which I instantly liked. I also found [reddit.com/r/minilab](reddit.com/r/minilab) which was useful to see what others had made. I had to stop scrolling and start. 
<br>
Knowing how to start was tricky. How do I use a switch to get VLANs set up? I started with setting up the GL.iNet Slate AX 1800 travel router. I used the repeater method. I also set up VPN through the travel router’s admin panel. Next was the switch. It wasn’t all that scary setting up VLANs. A few YouTube videos, reading and re-reading the Netgear documentation. I configured VLANs on the switch and via LuCl, OpenWrt for the router. Now I have two separate networks to use for my tech playground.

The mini lab took about one week to set up. I was determined to get it set up and not get too distracted or despondent when things didn’t come together the first time. It was on my To Do list for too long and needed to just get done. It’s been great to ‘raise the bar’ of my home network. But also get a win to build my confidence with doing something pretty technical. 

**Tips:**

* Take notes along the way. Having to search for Powershell commands or how to fix error messages a second time is annoying.
* It can be super frustrating. Being 95% way through and then some weird thing happens that you need to work out: trying other things to sort out a problem. But then it is so rewarding when it finally all comes together and works.
  
**11 July 2025**
I dug out a Raspberry Pi 2 and put Pi-hole on it. I have been meaning to set it up for ages. Was a fun little project. The wifi seems a bit sketchy. I might use the Raspberry Pi for something else and set up NextDNS instead.

**29 August 2025**
Back to setting up an analysis lab. Set up FLARE-VM.

**12 September 2025**
Taking FLARE-VM for a 🏎️ spin.

**Hardware:**
* 2 x Lenovo ThinkCentre M910q $199 x 2
* GL.iNet Slate AX (GL-AXT1800) $110
* Netgear 8 port managed switch $91
* CAT 6 Ultra Thin Ethernet Cables $12
* Total: $610.64

**Software:**
* Mullvad VPN $9/month
  
__________________

Sources: 
- [Joff Thyer, Black Hills Information Security, Pandemic Paradigm Shift Remote working *is* the New Normal](https://www.blackhillsinfosec.com/wp-content/uploads/2020/09/SLIDES_PandemicParadigmShift.pdf)

- [Kyle Cucci's Evasive Malware: Understanding Deceptive and Self-Defending Threats](https://nostarch.com/evasive-malware)

- [Dr Josh Stroschein - The Cyber Yeti, Building a VM for Reverse Engineering and Malware Analysis! Installing the FLARE-VM](https://youtu.be/i8dCyy8WMKY?si=fPyQ1IvwUlKwmISu)
