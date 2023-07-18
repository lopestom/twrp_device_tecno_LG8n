## After the twrp-12 branch has TWRP started in the device so WIP branch is for solving some issues.

### TWRP device tree for Tecno Pova 4 Pro (LG8n) - MT6789 - A12 

This branch android-12.1 has ***encrypt/decrypt*** files and option to more test with that. 

### Firmware version: LG8n-H891P-S-RU-230519V2407.zip -- LG8n-H891OPAeAf-S-GL-230519V1793
files individually from tester.

## Device

Specs [here](https://www.gsmarena.com/tecno_pova_4_pro-11925.php)
Description | Specification
-------:|:-------------------------
Shipped Android Version | 12
Internal Storage | 256 GB (UFS 2.1)

![Tecno Pova 4 Pro2](https://cdn-files.kimovil.com/default/0007/90/thumb_689602_default_big.jpg)

### Status

The tester only install `vendor_boot-LG8n-20230717.img` file to know if working.
<details><summary>History - Click to open</summary>
<p>
Some tests was made:

### Second img Test

* Initial DT: 2023-07-15
   Compiled img file 2023-07-16 and tested in 2023-07-17

- MT6789 - A12
  - Status: booted??
  - [X] booted

   - vendor_boot-LG8n-20230715.img => Working?? Not working?
  - [X] Working
  - [X] CPU/temperature correct
  - [X] Vibrator module not work

</p>
</details>

<details><summary>TWRP Pictures - Click to open</summary>
<p>

![Backup](https://github.com/lopestom/twrp_device_tecno_LG8n/releases/download/Tecno_Pova_4_Pro-LG8n_V2407/IMG_2023-07-18-18-34-28-764-WIP.jpg) ![Restore](https://github.com/lopestom/twrp_device_tecno_LG8n/releases/download/Tecno_Pova_4_Pro-LG8n_V2407/IMG_2023-07-18-18-34-03-829-WIP.jpg)

![Menu](https://github.com/lopestom/twrp_device_tecno_LG8n/releases/download/Tecno_Pova_4_Pro-LG8n/IMG_2023-07-17-23-20-01-920-TWRP-1.jpg)

![Install zip](https://github.com/lopestom/twrp_device_tecno_LG8n/releases/download/Tecno_Pova_4_Pro-LG8n/IMG_2023-07-18-00-17-13-924-TWRP-1.jpg)

![Install img](https://github.com/lopestom/twrp_device_tecno_LG8n/releases/download/Tecno_Pova_4_Pro-LG8n/IMG_2023-07-18-00-55-29-230-TWRP-1.jpg)

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
