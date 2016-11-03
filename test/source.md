class: split-30 nopadding
background-image: url( bkgs/daun.jpg )

.column_t2.center[.vmiddle[
.fgtransparent[
# .fa-3x.fa-stack[.red[<i class="fa icon-fire-alt fa-stack-2x"></i>]<i class="fa icon-wireless fa-stack-1x"></i>]
]
]]
.column_t2[.vmiddle.nopadding[
.shadelightdark[.boxtitle1[
### Pre-Title 6
# Sample Title

### [Eueung Mulyana](https://github.com/eueung)
### http://eueung.github.io/docker-stuff/rtl-sdr
#### CodeLabs | [Attribution-ShareAlike CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/)
#### 
]]
]]

---
class: column_t1 middle

.fonth4[
.tabtype1.fullwidth[
| Sample Outline  |
|:-------------:|
| Preparation |
| Google Radio Receiver |
| RTL-SDR with Docker |
| ... |
]]

---
class: split-30 nopadding
background-image: url( bkgs/batu.jpg )

.column_t2.center[.vmiddle[
.fgtransparent[
# .fa-3x.fa-stack[.red[<i class="fa icon-fire-alt fa-stack-2x"></i>]<i class="fa icon-wireless fa-stack-1x"></i>]
]
]]
.column_t2[.vmiddle.nopadding[
.shadelightdark[.boxtitle1[
### 
# Preparation

### 
### 
#### 
#### 
]]
]]

---
class: split-30 nopadding 

.column_t1[.vmiddle.pushfront.right[
# RPI
]]
.column_t2[.vmiddle[

```bash
*$ flash -c config.yaml -d /dev/mmcblk0 hypriotos-rpi-v0.8.0.img

*# config.yaml
hostname: node1
wifi:
  interfaces:
    wlan0:
      ssid: "lk8fm"
      password: "1234567890"

# ---
*$ sudo ./blacklist.sh 
*$ less /etc/modprobe.d/rtlsdr-blacklist.conf 

*# blacklist.sh - manually blacklist
#!/bin/bash

sudo echo -e "blacklist rtl2832\n\
blacklist r820t\n\
blacklist rtl2830\n\
blacklist dvb_usb_rtl28xxu" > /etc/modprobe.d/rtlsdr-blacklist.conf 
```

]]

---
class: column_t1  middle center

#Start .yellow[**rtl\_tcp**] Client &amp; Connect ...

.fonth5[
We're using [SDR\#](http://airspy.com/)<br/>
or any other rtl\_tcp-compatible clients ...
]

---
class: split-30 nopadding
background-image: url( bkgs/batu.jpg )

.column_t2.center[.vmiddle[
.fgtransparent[
# .fa-3x.fa-stack[.red[<i class="fa icon-fire-alt fa-stack-2x"></i>]<i class="fa icon-wireless fa-stack-1x"></i>]
]
]]
.column_t2[.vmiddle.nopadding[
.shadelightdark[.boxtitle1[
### 
# Refs

### 
### 
#### 
#### 
]]
]]

---
# Refs
.fonth5[
1. [Rtl_fm Guide: Updates for rtl_fm overhaul](http://kmkeen.com/rtl-demod-guide/)
1. [th0ma5w/rtl_fm_python: An API and web application to interact with a running instance of RTL_FM](https://github.com/th0ma5w/rtl_fm_python)
1. [google/radioreceiver: An application to listen to broadcast stereo FM and AM radio from your Chrome browser or your ChromeBook computer using a $15 USB digital TV tuner.](https://github.com/google/radioreceiver)
1. ...
]

---
class: split-30 nopadding
background-image: url( bkgs/daun.jpg )

.column_t2.center[.vmiddle[
.fgtransparent[
# .fa-3x.fa-stack[.red[<i class="fa icon-fire-alt fa-stack-2x"></i>]<i class="fa icon-wireless fa-stack-1x"></i>]
]
]]
.column_t2[.vmiddle.nopadding[
.shadelightdark[.boxtitle1[
### 
# END

### [Eueung Mulyana](https://github.com/eueung)
### http://eueung.github.io/docker-stuff/rtl-sdr
#### CodeLabs | [Attribution-ShareAlike CC BY-SA](https://creativecommons.org/licenses/by-sa/4.0/)
#### 
]]
]]

