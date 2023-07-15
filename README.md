# TWRP device tree for Tecno Pova 4 Pro (LG8n) - MT6789 - A12 

This branch android-12.1 has ***encrypt/decrypt*** files and option to more test with that. 

### Firmware version: LG8n-H891P-S-RU-230519V2407.zip -- LG8n-H891OPAeAf-S-GL-230519V1793
files individually from tester.

## Status

Specs [here](https://www.gsmarena.com/tecno_pova_4_pro-11925.php)
Description | Specification
-------:|:-------------------------
Shipped Android Version | 12
Internal Storage | 256 GB (UFS 2.1)

![Tecno Pova 4 Pro](https://cdn-files.kimovil.com/default/0007/90/thumb_689601_default_big.jpg)

![Tecno Pova 4 Pro2](https://cdn-files.kimovil.com/default/0007/90/thumb_689602_default_big.jpg)

![Tecno Pova 4 Pro3](https://fdn2.gsmarena.com/vv/pics/tecno/tecno-pova4-pro-1.jpg)

### First img Test

The tester only install `vendor_boot-LG8n-20230715.img` file to know if working.
<details><summary>History - Click to open</summary>
<p>
The first test.

### Some tests was made: 

* Initial DT: 2023-07-15
   Compiled img file 2023-07-15 and tested in 2023-07-16

- MT6789 - A12
  - Status: booted??
  - [?] booted

   - vendor_boot-LG8n-20230715.img => Working?? Not working?
  - [?] Working

</p>
</details>

<details><summary>TWRP Pictures - Click to open</summary>
<p>

![TWRP Touch screen fixed](https://github.com/lopestom/)

![TWRP Encryption/Decryption fixed](https://github.com/lopestom/)
</p>
</details>

#### Big thanks to:

- [Serega77plus from 4pda](https://4pda.to/forum/index.php?showuser=5528632)
- [TeamWin](https://github.com/TeamWin) for TWRP SC.
* TWRP version 3.7.0_12 *

                  ####### generated by lopestom #######
-----
#### flashing

```bash
fastboot
fastboot flash vendor_boot_[a][b] vendor_boot.img
```

-----
#### Building

```bash
export ALLOW_MISSING_DEPENDENCIES=true
export LC_ALL=C
export USE_NINJA=false
. build/envsetup.sh
lunch twrp_LG8n-eng
mka vendorbootimage
```
