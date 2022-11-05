# 🦊 OrangeFox Recovery CI
A Free CI to Build OrangeFox Recovery From GitHub's Workflow.
***
## How to Use this Workflow ?
### - Fork and Build

**Note:** **Read this table carefully and change the variables in `get_fox_recovery.sh` script file according to your need.**
Variable's Name | Defaults | Variables
----- | ----- | -----
`FOX_BRANCH` | default is `fox_12.1` | fox_9.0, fox_10.0, fox_11.0, fox_12.1 ?
`TWRP_BRANCH` | default is `twrp-12.1` | twrp-9.0, twrp-10.0, twrp-11.0, twrp-12.1 ?
`TWRP_MIN_MANIFEST` | default is `aosp` | aosp, omni ?
`DEVICE_BRANCH` | default is `fox_12.1` | it can be anything, may be fox_12.1
`OEM` | default is `xiaomi` | xiaomi,samsung,etc ?
`DEVICE_TREE_URL` | `https://gitlab.com/OrangeFox/device/miatoll.git` | your device tree URL ?
`LOCAL_DEVICE_TREE_URL` | `git@gitlab.com:OrangeFox/device/miatoll.git` | your local device tree URL ?
`FOX_VENDOR_BRANCH` | default is `fox_12.1` | master, fox_10.0, fox_11.0, fox_12.1 ?
`test_build_device` | default is `miatoll` | codename of your device ?
`FOX_OMNI_DEVICE` | default is `0` (is your device OMNI then, change this to `1`) | `0` & `1` ?
`FOX_AOSP_DEVICE` | default is `0` (is your device AOSP then, change this to `1`) | `0` & `1` ?
`FOX_OMNI_VAB_DEVICE` | default is `0` (is your device OMNI & A/B then, change this to `1`) | `0` & `1` ?
`FOX_AOSP_VAB_DEVICE` | default is `1` (is your device AOSP & A/B then, change this to `1`) | `0` & `1` ?

### - Steps for running this workflow :

* Fork this [repository](https://github.com/Diwas1111/Recovery-Builder) giving whatever name you want.
* Go to `get_fox_recovery.sh` script file & change the variable name's default value using `Variables` from the table <br> **Note:** **`get_fox_recovery.sh` this script file compiles recovery for `miatoll` by default so, you need to change variables according to your need.** </br>
* Go to `Actions` tab and select the workflow named `Recovery Builder`.
* Click `Run Workflow` button on the left of `This workflow has a workflow_dispatch event trigger` line.
* And that's it ! , to download the build see your Action's logs.
***

## Credits
- [Sushrut1101](https://github.com/Sushrut1101) - For Helping
- [Mikubill](https://github.com/Mikubill) - For [this](https://github.com/Mikubill/transfer)
- [sarthakroy2002](https://github.com/sarthakroy2002) - For `android_build_env.sh` Script File
- [OrangeFox](https://gitlab.com/OrangeFox) - For Base Script File
- [TeamWin](https://github.com/TeamWin) - For Sources
- [Diwas007](https://github.com/Diwas007) - For Making This Happen
- And Many More!

# License

        Copyright (c) 2022 Diwas007

       Licensed under the Apache License, Version 2.0 (the "License");
       you may not use this file except in compliance with the License.
       You may obtain a copy of the License at

          http://www.apache.org/licenses/LICENSE-2.0

       Unless required by applicable law or agreed to in writing, software
       distributed under the License is distributed on an "AS IS" BASIS,
       WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
       See the License for the specific language governing permissions and
       limitations under the License.
