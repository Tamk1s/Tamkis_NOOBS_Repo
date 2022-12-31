# Tamkis_NOOBS_Repo
Central online image source repository for custom [NOOBS](https://www.raspberrypi.org/downloads/noobs/)/[PINN](https://github.com/procount/pinn)-compatible Raspberry Pi distro images that I roll from stock images.
 
**Current OS images hosted by these JSON files:**
- [DreamPi DX](https://sourceforge.net/projects/dreampi-noobs/)
  - 2 variants of image
    - DreamPi for Raspberry Pi 1-3, Zero
	- DreamPi for Raspberry Pi 4 and newer
  - Image variants modified from stock DreamPi image (v1.7 DLE) with various community addon patches
	- DreamPi Netlink Tunneler for Netlink (Sega Saturn)
	  - Allows for web browsing, Netlink Zone/features, dialup gameplay for applicable Sega Saturn Netlink/XBand/modem games
	  - [Sega Saturn VOIP Guide](https://dreamcast-talk.com/forum/viewtopic.php?t=8453)
	  - [DreamPi Netlink Tunneler patch](https://github.com/eaudunord/Netlink/)
	- Dreamcast Now for BBA
	  - Allows DreamPi to appear on [Dreamcast Now](https://dreamcast.online/now/) service when using a BBA connection
	  - [DC Now BBA patch](https://www.dreamcast-talk.com/forum/viewtopic.php?f=3&t=14233)
	- Wi-Fi to Ethernet bridge (BBA)
	  - If the DreamPi is using WiFi connection for internet and Dreamcast is using a BBA, allows to repeat/bridge highspeed broadband connection to the Dreamcast
	  - [WiFi/Ethernet bridge patch](https://dreamcast-talk.com/forum/viewtopic.php?f=3&t=15845)
- [XBandPi](https://sourceforge.net/projects/xbandpi-noobs/)
  - 2 variants of image
    - XBandPi for Raspberry Pi 1-3, Zero (based on stock DreamPi image)
	- XBandPi for Raspberry Pi 4 and newer (based on stock DreamPi4 image)
- [XLink Kai](https://sourceforge.net/projects/xlink-kai-noobs/) (**NOT FUNCTIONAL**)

**These repositories are setup as such:**
- All assets for generation/defintition of the image (marketing slide_vga source images, JSON files defining partitions and general OS data)
- Tarballs
  - Marketing.tar (slide_vga images)
  - boot.tar.xz (boot partition image)
  - root.tar.xz (root partition image)
  - These tarballs are stored the respective Sourceforge repos.
     - Tarballs need server/internet raw file access, and are usually >=100MB in size
	 - Otherwise would otherwise require pesky Git LFS/quota support on Github

**This repository contains:**
- repo_list.json
  - Lists of tables to OS distros.
  - Contains 1 entry, points to os_list_v3.json
- os_list_v3.json
  - Lists of all distro images and accompanying data.
  - They point to various JSOn, image, and other data assets online from the respective OS distro repository

Please read the [PINN](https://github.com/procount/pinn) repository for full information on these 2 types of JSON files.
General technical information on how to setup a NOOBS image for online server support available on the [DreamPi NOOBS page](https://www.eaglesoftltd.com/retro/dc/dreampi-noobs)