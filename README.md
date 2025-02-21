# Tamkis_NOOBS_Repo
Central online image source repository for custom [NOOBS](https://www.raspberrypi.org/downloads/noobs/)/[PINN](https://github.com/procount/pinn)-compatible Raspberry Pi distro images that I roll from stock images.
 
**Current OS images hosted by these JSON files:**
- [DreamPi DX](https://sourceforge.net/projects/dreampi-noobs/) v1.3 (v1.9 DLE)
  - **2 variants of image**
    - DreamPi for Raspberry Pi 1-3, Zero
	- DreamPi for Raspberry Pi 4 and newer
  - Latest stock DreamPi image (**v1.9 DLE**) with various community addon patches included
	- [**BBA Mode for DreamPi**](https://dreamcast-talk.com/forum/viewtopic.php?f=3&t=16649)
	  - Allows DreamPi to appear on [Dreamcast Now](https://dreamcast.online/now/) service when using a BBA connection
	  - **Wi-Fi to Ethernet bridge (BBA)**
        - If the DreamPi is using WiFi connection for internet and Dreamcast is using a BBA, allows to repeat/bridge highspeed broadband connection to the Dreamcast
	- **DreamPi Netlink Tunneler for Netlink (Sega Saturn)**
	  - Allows for web browsing, Netlink Zone/features, dialup gameplay for applicable Sega Saturn Netlink/XBand/modem games
	  - [Sega Saturn VOIP Guide](https://dreamcast-talk.com/forum/viewtopic.php?t=8453)
	  - [DreamPi Netlink Tunneler patch](https://github.com/eaudunord/Netlink/)
	- **[XBAND 16-bit](https://xband.retrocomputing.network/) support (Sega Genesis, SNES/SFC)**
	  - X-Mail (cross-platform on Gen/SNES supported, not yet supported on SFC)
	  - BANDWIDTH
	  - XBAND News
	  - Player Lists (cross-platform on Gen/SNES supported)
	  - Gameplay (on DreamPi only, for supported games)
- [XBandPi](https://sourceforge.net/projects/xbandpi-noobs/) (**OBSOLETE, please use latest DreamPi DX image**)
- [XLink Kai](https://sourceforge.net/projects/xlink-kai-noobs/) (**NOT FUNCTIONAL**)

**These repositories are setup as such:**
- All assets for generation/defintition of the image (marketing slide_vga source images, JSON files defining partitions and general OS data)
- **Tarballs**
  - Marketing.tar (slide_vga images)
  - boot.tar.xz (boot partition image)
  - root.tar.xz (root partition image)
  - These tarballs are stored the respective Sourceforge repos.
     - Tarballs need server/internet raw file access, and are usually >=100MB in size
	 - Otherwise would otherwise require pesky Git LFS/quota support on Github

**This repository contains:**
- **repo_list.json**
  - Lists of tables to OS distros.
  - Contains 1 entry, points to os_list_v3.json
- **os_list_v3.json**
  - Lists of all distro images and accompanying data.
  - They point to various JSON, image, and other data assets online from the respective OS distro repository

Please read the [PINN](https://github.com/procount/pinn) repository for [full information](https://github.com/procount/pinn/wiki/JSON-fields) on these 2 types of JSON files.
General technical information on [how to setup](https://github.com/procount/pinn/wiki/How-to-Create-a-Multi-Boot-SD-card-out-of-2-existing-OSes-using-PINN) a NOOBS image for online server support available on the [DreamPi NOOBS page](https://www.eaglesoftltd.com/retro/dc/dreampi-noobs)