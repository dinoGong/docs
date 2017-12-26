###bluetooth

```
apt install bluez bluez-hcidump -y -f
```

```
lsusb
```

```
Bus 001 Device 002: ID 8087:8000 Intel Corp. 
Bus 001 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub
Bus 003 Device 001: ID 1d6b:0003 Linux Foundation 3.0 root hub
Bus 002 Device 002: ID 17ef:6050 Lenovo 
Bus 002 Device 009: ID 05c6:9039 Qualcomm, Inc. 
Bus 002 Device 005: ID 04f2:b469 Chicony Electronics Co., Ltd 
Bus 002 Device 004: ID 04ca:300b Lite-On Technology Corp. Atheros AR3012 Bluetooth
Bus 002 Device 003: ID 06cb:2970 Synaptics, Inc. touchpad
Bus 002 Device 001: ID 1d6b:0002 Linux Foundation 2.0 root hub
```


```
lsusb -s 002:004 -v
```

```
AR3012
```

```
git clone git://git.kernel.org/pub/scm/linux/kernel/git/firmware/linux-firmware.git
```

```
wget http://ftp.cn.debian.org/debian/pool/non-free/f/firmware-nonfree/firmware-atheros_0.36+wheezy.1_all.deb
```

```
dpkg -i firmware-atheros_0.36+wheezy.1_all.deb
```

```
reboot
```

```
hciconfig -a
hci0:	Type: Primary  Bus: USB
	BD Address: 5C:93:A2:79:8A:6A  ACL MTU: 1022:8  SCO MTU: 183:5
	UP RUNNING 
	RX bytes:736 acl:0 sco:0 events:57 errors:0
	TX bytes:5128 acl:0 sco:0 commands:57 errors:0
	Features: 0xff 0xfe 0x0d 0xfe 0xd8 0x7f 0x7b 0x8f
	Packet type: DM1 DM3 DM5 DH1 DH3 DH5 HV1 HV2 HV3 
	Link policy: RSWITCH HOLD SNIFF 
	Link mode: SLAVE ACCEPT 
	Name: 'debian'
	Class: 0x1c010c
	Service Classes: Rendering, Capturing, Object Transfer
	Device Class: Computer, Laptop
	HCI Version: 4.1 (0x7)  Revision: 0x3101
	LMP Version: 4.1 (0x7)  Subversion: 0x1
	Manufacturer: Atheros Communications, Inc. (69)

```

```
hcitool lescan
LE Scan ...
4F:08:23:0E:D5:33 (unknown)
2E:CA:0E:8B:21:1E (unknown)
A4:5E:60:E7:9D:40 (unknown)
67:F0:CE:9C:B4:ED (unknown)
67:F0:CE:9C:B4:ED (unknown)
4D:DE:CF:11:C5:CA (unknown)
64:09:80:6F:18:84 (unknown)
6D:DB:A8:BF:63:79 (unknown)
4F:08:23:0E:D5:33 (unknown)
67:F3:52:83:A7:99 (unknown)
58:5A:69:C7:0B:FB (unknown)
34:36:3B:CD:E6:E9 (unknown)

```
