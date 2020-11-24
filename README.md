# Meek-Modules

All modules connected to a 2.4GHz Wifi Connection.
The Wifi connection has been setup in router as follow:

Im using a Asus ROG Rapture GT-AX11000 Router

Enable Smart Control: off
802.11ax / Wi-Fi 6 mode: enable (didn't try to disable if this will be better)
Wi-Fi Agile Multiband: disable
Target Wake Tim: enable
Channel Bandwidth: 20 MHz
Control Channel: 11 (seems that higher or lower give connection problems)
Auth Method: WPA/WPA-2 Personal
WPA Encryption: TKIP+AES
Protect Management Frame: disable
Group Key Rotation Interval: 3600

GPIO Schema:

MP1:
  Touch1:       GPIO13
  Dopplet:      GPIO 12
  Output 1:     GPIO 5
  Speaker:      GPIO 15
  RGB Led:      GPIO 2
  Touch Power:  GPIO 16

MT1:
  Touch1:       GPIO 12
  Output 1:     GPIO 5
  Speaker:      GPIO 0
  RGB Led:      GPIO 2
  Touch Power:  GPIO 16

MT2:
  Touch1:       GPIO 12
  Touch2:       GPIO 13     
  Output 1:     GPIO 5
  Output 2:     GPIO 4
  Speaker:      GPIO 0
  RGB Led:      GPIO 2
  Touch Power:  GPIO 16

MT3:
  Touch1:       GPIO 14
  Touch2:       GPIO 12
  Touch3:       GPIO 13
  Output 1:     GPIO 5
  Output 2:     GPIO 4
  Output 3:     GPIO 15
  Speaker:      GPIO 0
  RGB Led:      GPIO 2
  Touch Power:  GPIO 16  
