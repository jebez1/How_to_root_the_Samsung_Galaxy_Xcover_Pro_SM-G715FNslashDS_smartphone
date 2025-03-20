https://www.samsung.com/ae/business/smartphones/xcover/galaxy-xcover-pro-g715-sm-g715fzkdxsg/

Softwares used:
Bifrost
Magisk
Heimdall

PC OS here:
Arch Linux KDE

PC:                                                                                                                                   Smartphone:
Install https://aur.archlinux.org/packages/bifrost-bin                                                                                Settings
                                                                                                                                      About phone
Bifrost                                                                                                                               Software information
Model: SM-G715FN (SM-G715FN/DS worked not, DS stands for Dual SIM)                                                                    Tap 7 times Build number to unlock Developer options
Region: XEF (France for me, knew by https://github.com/zacharee/SamloaderKotlin?tab=readme-ov-file#how-do-i-know-which-csc-to-use)    Settings
Serial: R58N416YJDP (knew by smartphone, Settings, About phone)                                                                       Developer options
Check for Updates                                                                                                                     OEM unlocking
Download                                                                                                                              Power off
                                                                                                                                      Press volume up & down
SM-G715FN_4_20240130132110_y912sb1jdi_fac_G715FNXXSDFXA1_G715FNOXMDFXA1_G715FNXXSDFXA1_G715FNXXSDFXA1_XEF.zip                         Plug the smartphone as USB to a PC
    AP_G715FNXXSDFXA1_QB76687873_REV00_user_low_ship_meta_OS13.tar.md5                                                                Volume up long press (Device unlock mode)
        boot.img.lz4                                                                                                                  Volume up (Unlock bootloader)
            boot.img                                                                                                                  Reinstall Android
                                                                                                                                      Download Magisk https://github.com/topjohnwu/Magisk/releases
                                                                                                                                      Install it
Upload boot.img to the smartphone by USB

Smartphone:
Magisk
Install
Select and Patch a File
boot.img
Upload Downloads/magisk_patched-28102_jXp8V.img to the PC by USB

PC:                                                                                                                                    Smartphone:
Rename magisk_patched-28102_jXp8V.img to boot.img                                                                                      Power off
                                                                                                                                       Press volume up & down
sudo pacman -S heimdall                                                                                                                Plug the smartphone as USB to a PC
                                                                                                                                       Volume up (Continue)
heimdall flash --BOOT a_path/boot.img

Smartphone:
Restore factory configuration
Reinstall modified Android
Reinstall Magisk

The end.

E.g. root adb shell:
Smartphone:
Settings
Developer options
USB debugging
PC:
adb shell
Smartphone:
Magisk
Superuser
Set Shell on
PC:
su
