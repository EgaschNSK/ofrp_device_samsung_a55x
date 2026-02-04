# OrangeFox 12.1 for Samsung Galaxy A55 5G SM-A556E (a55x)

![Test Image 7](https://gitlab.com/uploads/-/system/group/avatar/2810739/256.png?width=256)

## Flash Steps
Assuming you know the basic of flashing...
* Via ZIP Installer
    * Download `OrangeFox-R11.3_1-Stable-a55x.zip` file on orangefox.download.
    * Reboot your device to OFRP/TWRP, and flash zip.
    * Reboot now to Recovery.

## Build Steps
Assuming you know the basic of preparing build environment...
* Prepare and Sync OrangeFox Source:
```
mkdir ~/OrangeFox_sync
cd ~/OrangeFox_sync
git clone https://gitlab.com/OrangeFox/sync.git # (or, using ssh, "git clone git@gitlab.com:OrangeFox/sync.git")
cd ~/OrangeFox_sync/sync/
./orangefox_sync.sh --branch 12.1 --path ~/fox_12.1
```
* goto Directory
```
cd ~/fox_12.1
```
* Device Tree (Make sure you are in root directory of Orangefox Source.):
```
git clone https://gitlab.com/egaschnsk/ofrp_device_samsung_a55x -b fox12_1 ./device/samsung/a55x
```
* Build (Make sure you are in root directory of OrangeFox source.)
```
source build/envsetup.sh; export ALLOW_MISSING_DEPENDENCIES=true; lunch twrp_a55x-eng; mka vendorbootimage
```
# Done! Check / find `OrangeFox-R11.3_1-Stable-a55x.zip` in `out/target/product/a55x/target/product/a55x/´ directory.
