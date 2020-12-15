# Tamkis_NOOBS_Repo
Central online image source repository for custom [NOOBS](https://www.raspberrypi.org/downloads/noobs/)/[PINN](https://github.com/procount/pinn)-compatible Raspberry Pi distro images I roll from stock images.
 
**Current OS images hosted by these JSON files:**
- [DreamPi](https://sourceforge.net/projects/dreampi-noobs/)
- [XLink Kai](about:blank)

**These repositories are setup as such:**
- All assets for generation/defintition of the image (marketing slide_vga source images, JSON files defining partitions and general OS data)
- Tarballs
  - Marketing.tar (slide_vga images)
  - boot.tar.xz (boot partition image)
  - root.tar.xz (root partition image)
  - These tarballs are stored elsewhere online. (It needs server/internet raw file access, and are usually >=100MB in size, which would otherwise require pesky Git LFS/quota support.)

**This repository contains:**
- repo_list.json
  - Lists of tables to OS distros.
  - Contains 1 entry, points to os_list_v3.json
- os_list_v3.json
  - Lists of all distro images and accompanying data.
  - They point to various JSOn, image, and other data assets online from the respective OS distro repository

Please read the [PINN](https://github.com/procount/pinn) repository for full information on these 2 types of JSON files.