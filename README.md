## OrangeFox Recovery device tree for the Samsung Galaxy A55 5G (Exynos)

The Galaxy A55 5G (SM-A556E - codenamed _"a55x"_) is an upper-mid-range smartphone from Samsung.

It was announced in March 2024 and released in March 2024.

## Device specifications

| Feature                        | Specification                                                                             |
| -----------------------------: | :---------------------------------------------------------------------------------------- |
| Chipset                        | Exynos 1480 (4 nm)                                                                        |
| CPU                            | Octa-core (4x2.7 GHz Cortex-A78 & 4x2.0 GHz Cortex-A55)                                   |
| GPU                            | Xclipse 530                                                                               |
| Memory                         | 8GB / 12GB RAM                                                                            |
| Shipped OS                     | Android 14 (One UI 6.1)                                                                   |
| Storage                        | 128GB / 256GB                                                                             |
| SIM                            | Nano-SIM + eSIM or Dual SIM (varies by region)                                            |
| MicroSD                        | microSDXC (uses shared SIM slot)                                                          |
| Battery                        | Li-Ion 5000 mAh (non-removable), 25W fast charge                                          |
| Dimensions                     | 161.1 x 77.4 x 8.2 mm                                                                     |
| Display                        | 6.6 inches, 1080 x 2340, 19.5:9 ratio (~390 ppi), Super AMOLED, 120Hz                     |

## Device picture

<img src="https://fdn2.gsmarena.com/vv/pics/samsung/samsung-galaxy-a55-1.jpg" width="45%"/>

---
# Flashing
## Flashing with an installed custom recovery (OrangeFox/TWRP):
    * Download the OrangeFox zip installer file from orangefox.download
    * Reboot your device to your custom recovery
    * Flash the OrangeFox zip installer (there will be an automatic reboot to OrangeFox after flashing)

##  Flashing with Odin:
    * Download the OrangeFox zip installer file from orangefox.download
    * Extract the OrangeFox "img.tar" file from the zip installer
    * Open Odin
    * Reboot the device to download mode
    * Flash the "img.tar" file to the "AP" slot in Odin
    * Reboot to recovery, using the relevant hardware key combination
    * If flashing a custom recovery for the very first time on OneUI, you *must* now *format* your data partition:
        * Go to Wipe -> Format Data -> type "Yes", and swipe
        * Reboot to System and configure the Android ROM
    * Reboot to OrangeFox and flash the OrangeFox zip installer

---
## Copyright

```
#
# Copyright (C) 2026 The TWRP Open Source Project
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
#  *  Copyright (C) 2026 The OrangeFox Recovery Project
#  *
#  * This program is free software: you can redistribute it and/or modify
#  * it under the terms of the GNU General Public License as published by
#  * the Free Software Foundation, either version 3 of the License, or
#  * (at your option) any later version.
#  *
#  * This program is distributed in the hope that it will be useful,
#  * but WITHOUT ANY WARRANTY; without even the implied warranty of
#  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
#  * GNU General Public License for more details.
#  *
#  * You should have received a copy of the GNU General Public License
#  * along with this program.  If not, see <http://www.gnu.org/licenses/>.
#
```
