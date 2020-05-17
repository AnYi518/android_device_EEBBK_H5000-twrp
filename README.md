TWRP device tree for EEBBK H20 (codenamed "H5000")
===============

Basic        | Spec Sheet
------------:|:------------------------
CPU          | Cortex-A35 | Hexa-Core | MT8167
GPU          | PowerVR GE8300
Memory       | 2GB RAM
Shipped Android Version | 7.0
Storage      | 32GB
Battery      | 6000 mAh Li-Po
Display      | 10.1 inch
Rear Camera  | 5.0 MP
Front camera | 2.0 MP

This branch is for building TWRP.

### To build: 

```
$ mkdir twrp

$ cd twrp

$ repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-7.1

To initialize a shallow clone, which will save even more space, use a command like this:

$ repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-7.1

After that sync your sources:

$ repo sync

Download or clone this repository, go to /twrp/device and create EEBBK/*. Copy this repo to your created folder

Build your recovery:

$ source build/envsetup.sh

& lunch *-eng

make clean && make recoveryimage
```
