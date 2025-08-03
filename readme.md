# Project  S3 Trio64 VLB  video card
It was developement from Project S3 ViRGE VLB   to switching into Trio64 Mode instead  LFB-Mode (which it is requiered by VIRGE VLB )
https://github.com/matt1187/765VL

![grafik](https://github.com/matt1187/764VL/assets/155289528/fb30cfb3-c5dd-4119-bc6e-0a928e994fff)


# PCB Revision History  (attention, two PCB type )
- 325VL-000 initial draft
- 764VL-000 spinoff of 325VL-000 included bug fixing (DDC interface, config strap ), removed discrete adress decoder, added VAFC
- 764VL-001 minor bug fixing (swapped VGA footprint, reversed LED )

# Feartures
- S3 Trio64 video chipset
- one of last S3 Videochip for VLB without buggy VLB (Trio64V+ has buggy VLB interface)
- really fast video card for VESA local bus platform. (only ARK 1000VL and Trio64V+ is faster in DOS)
- 2 MB DRAM
- 135 MHz integrated RAMDAC
- VESA feartures connector (not tested )
- DDC2B interface
- rock solid  40 MHz bus-clock with zero wait-state
- Win 3.1, Win9x, Win NT 3.51 & 4 driver available
- cheap Trio64 PCI card as component-donor.
- cheap 2 layer platine layout (and stable up to 90 MHz DRAM clock with S3 ViRGE ) NOTEICE: Reused 325VL-Layout with modification for VAFC.
  
# Issues 
- (need to verify) 50 MHz bus-clock -> RAMDAC isn't capable to handle of high clock (graphic artifact in DOOM). Except this issues,  video card is stable.
- (need to verify) 765VL doesn't work with Alaris Leopard (486SLC2 Motherboard) 
- small SOJ-40 footprint requires good solder skill. (It works fine with stencil )
- no official S3 VBE 2.0  with linear framebuffer support. (it requires modification of S3VBE318.EXE)

Quote of mkarcher "As S3VBE20 is not "free/open source software", I don't have a license to modify it, to run modified versions, and certainly not to distribute modified versions, though. If you want to take the legal risk yourself, get S3VBE/Core 2.0 version 3.18, understand that the terms of use explicitly state that the license for using, copying and distributing only applies "if you don't modify the files in this package in any way", so you certainly wouldn't undo the LZEXE compression, and patch the byte at offset 0x2d2f from 0x75 to 0xEB."

# notes

# bill material

- [![csv-file ](https://github.com/matt1187/764VL/blob/main/Gerber/764VL-001.csv)]
- [![gerber-file ](https://github.com/matt1187/764VL/blob/main/Gerber/764VL-001.zip)]

 # License
The project is free for non-commercial reproduction. Do not sell it on Ebay or other platforms for profit. Do not make a closed source derivative. Share your experiences and ideas with the community.

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png

