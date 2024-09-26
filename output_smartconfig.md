I (31) boot: ESP-IDF v5.3-dirty 2nd stage bootloader
I (31) boot: compile time Sep 26 2024 15:23:58
I (31) boot: Multicore bootloader
I (36) boot: chip revision: v3.0
I (40) boot.esp32: SPI Speed      : 40MHz
I (44) boot.esp32: SPI Mode       : DIO
I (49) boot.esp32: SPI Flash Size : 2MB
I (53) boot: Enabling RNG early entropy source...
I (59) boot: Partition Table:
I (62) boot: ## Label            Usage          Type ST Offset   Length
I (70) boot:  0 nvs              WiFi data        01 02 00009000 00006000
I (77) boot:  1 phy_init         RF data          01 01 0000f000 00001000
I (84) boot:  2 factory          factory app      00 00 00010000 00100000
I (92) boot: End of partition table
I (96) esp_image: segment 0: paddr=00010020 vaddr=3f400020 size=20c10h (134160) map
I (151) esp_image: segment 1: paddr=00030c38 vaddr=3ffb0000 size=03e58h ( 15960) load
I (157) esp_image: segment 2: paddr=00034a98 vaddr=40080000 size=0b580h ( 46464) load
I (175) esp_image: segment 3: paddr=00040020 vaddr=400d0020 size=8db58h (580440) map
I (374) esp_image: segment 4: paddr=000cdb80 vaddr=4008b580 size=0bc70h ( 48240) load
I (405) boot: Loaded app from partition at offset 0x10000
I (405) boot: Disabling RNG early entropy source...
I (417) cpu_start: Multicore app
I (425) cpu_start: Pro cpu start user code
I (426) cpu_start: cpu freq: 160000000 Hz
I (426) app_init: Application information:
I (428) app_init: Project name:     smart_config
I (434) app_init: App version:      1
I (438) app_init: Compile time:     Sep 26 2024 15:23:52
I (444) app_init: ELF file SHA256:  f42c6a6bb...
I (449) app_init: ESP-IDF:          v5.3-dirty
I (455) efuse_init: Min chip rev:     v0.0
I (459) efuse_init: Max chip rev:     v3.99 
I (464) efuse_init: Chip rev:         v3.0
I (469) heap_init: Initializing. RAM available for dynamic allocation:
I (476) heap_init: At 3FFAE6E0 len 00001920 (6 KiB): DRAM
I (482) heap_init: At 3FFB82A8 len 00027D58 (159 KiB): DRAM
I (489) heap_init: At 3FFE0440 len 00003AE0 (14 KiB): D/IRAM
I (495) heap_init: At 3FFE4350 len 0001BCB0 (111 KiB): D/IRAM
I (501) heap_init: At 400971F0 len 00008E10 (35 KiB): IRAM
I (509) spi_flash: detected chip: generic
I (512) spi_flash: flash io: dio
W (516) spi_flash: Detected size(4096k) larger than the size in the binary image header(2048k). Using the size in the binary image header.
I (530) main_task: Started on CPU0
I (540) main_task: Calling app_main()
I (570) wifi:wifi driver task: 3ffc025c, prio:23, stack:6656, core=0
I (580) wifi:wifi firmware version: 0caa81945
I (580) wifi:wifi certification version: v7.0
I (580) wifi:config NVS flash: enabled
I (580) wifi:config nano formating: disabled
I (580) wifi:Init data frame dynamic rx buffer num: 32
I (590) wifi:Init static rx mgmt buffer num: 5
I (590) wifi:Init management short buffer num: 32
I (600) wifi:Init dynamic tx buffer num: 32
I (600) wifi:Init static rx buffer size: 1600
I (610) wifi:Init static rx buffer num: 10
I (610) wifi:Init dynamic rx buffer num: 32
I (610) wifi_init: rx ba win: 6
I (620) wifi_init: accept mbox: 6
I (620) wifi_init: tcpip mbox: 32
I (620) wifi_init: udp mbox: 6
I (630) wifi_init: tcp mbox: 6
I (630) wifi_init: tcp tx win: 5760
I (640) wifi_init: tcp rx win: 5760
I (640) wifi_init: tcp mss: 1440
I (640) wifi_init: WiFi IRAM OP enabled
I (650) wifi_init: WiFi RX IRAM OP enabled
I (650) phy_init: phy_version 4830,54550f7,Jun 20 2024,14:22:08
I (730) wifi:mode : sta (94:b5:55:f6:f5:90)
I (730) wifi:enable tsf
I (730) main_task: Returned from app_main()
I (790) smartconfig: SC version: V3.0.1
I (5630) wifi:ic_enable_sniffer
I (5630) smartconfig: Start to find channel...
I (5630) smartconfig_example: Scan done
I (13660) smartconfig: TYPE: ESPTOUCH
I (13660) smartconfig: Found channel on 11-0. Start to get ssid and password...
I (13660) smartconfig_example: Found channel
I (15230) smartconfig: TYPE: ESPTOUCH
I (15230) smartconfig: T|AP MAC: 30:0a:c5:9e:94:9f
I (18910) smartconfig: F|pswd: 50769475
I (18910) smartconfig: F|ssid: AIS 4G Hi-Speed Home WiFi_76947550769475
I (18910) smartconfig: F|bssid: 30:0a:c5:9e:94:9f
I (18920) wifi:ic_disable_sniffer
I (18920) smartconfig_example: Got SSID and password
I (18920) smartconfig_example: Set MAC address of target AP: 30:0a:c5:9e:94:9f 
I (18930) smartconfig_example: SSID:AIS 4G Hi-Speed Home WiFi_769475
I (18940) smartconfig_example: PASSWORD:50769475
I (19260) wifi:new:<11,0>, old:<11,0>, ap:<255,255>, sta:<11,0>, prof:1, snd_ch_cfg:0x0
I (19260) wifi:state: init -> auth (0xb0)
I (19270) wifi:state: auth -> assoc (0x0)
I (19280) wifi:state: assoc -> run (0x10)
I (19290) wifi:connected with AIS 4G Hi-Speed Home WiFi_769475, aid = 16, channel 11, BW20, bssid = 30:0a:c5:9e:94:9f
I (19290) wifi:security: WPA2-PSK, phy: bgn, rssi: -57
I (19310) wifi:pm start, type: 1

I (19320) wifi:dp: 1, bi: 102400, li: 3, scale listen interval from 307200 us to 307200 us
I (19320) wifi:AP's beacon interval = 102400 us, DTIM period = 1
I (20320) esp_netif_handlers: sta ip: 192.168.1.119, mask: 255.255.255.0, gw: 192.168.1.1
I (20320) smartconfig_example: WiFi Connected to ap
I (20590) wifi:<ba-add>idx:0 (ifx:0, 30:0a:c5:9e:94:9f), tid:0, ssn:4, winSize:64
I (23390) smartconfig_example: smartconfig over
I (28440) wifi:<ba-add>idx:1 (ifx:0, 30:0a:c5:9e:94:9f), tid:6, ssn:0, winSize:64
