# Tamkis_NOOBS_Repo
Central online image source repository for custom [NOOBS](https://www.raspberrypi.org/downloads/noobs/)/[PINN](https://github.com/procount/pinn)-compatible Raspberry Pi distro images I roll from stock images.
 
**Current OS images hosted by these JSON files:**
- [DreamPi](https://sourceforge.net/projects/dreampi-noobs/)
  - 2 variants of image
    - DreamPi for Raspberry Pi 1-3, Zero
	- DreamPi for Raspberry Pi 4 and newer
- [XLink Kai](https://sourceforge.net/projects/xlink-kai-noobs/upload/)

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
General technical information on how to setup a NOOBS image for online server support available on the my [DreamPi NOOBS page](http://www.eaglesoftltd.com/retro/dc/dreampi-noobs)