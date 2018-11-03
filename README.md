## CloverEFIforN5110 ##

### Postinstall EFI folder for 10.11.6 and DELL N5110 only.

Resources are from insanelymac.com and tonymacx86.com.

More information about Clover on https://clover-wiki.zetam.org/Home.

## Notes
Use Clover to simulate EFI booting on DELL N5110 which owns legacy bios .

Clover version: r3923

System: Windows10 & El Capitan 10.11.6

Boot sequence:  BIOS-> MBR(boot0xx, here is boot0ss for dual system) -> PBR(bootx, here is boot6 for 64bit Clover bootloader) -> CloverX64.efi -> boot.efi(MAC) or bootmgr.efi (WINDOWS)-> OS

##### PS: So 'PBR multiple boot options' and 'boot0ss'(or boot0af which is up to your demand,see more on https://clover-wiki.zetam.org/Installation) msut be checked. These options are installed directly to the MBR of a disk(very begining of a disk), so unless you erase the disk, these options will keep staying on MBR.

##### 'APPLE' folder under EFI folder is to make Clover work.

##### No 'WINDOWS' folder under EFI folder here cause after installing Win correctly, WINDOWS folder would be added to your EFI partition,under EFI folder on that partition automatically.



