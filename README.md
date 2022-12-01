# Meek-Modules

All modules connected to a 2.4GHz Wifi Connection.
The Wifi connection has been setup in router as follow:

Im using a Asus ROG Rapture GT-AX11000 Router

- Enable Smart Control: off
- 802.11ax / Wi-Fi 6 mode: enable (didn't try to disable if this will be better)
- Wi-Fi Agile Multiband: disable
- Target Wake Tim: enable
- Channels NOT USE: 13, 14 and 15
- Channel Bandwidth: 20/40 MHz
- Control Channel: 11 (seems that higher or lower give connection problems)
- Auth Method: WPA/WPA-2 Personal
- WPA Encryption: TKIP+AES
- Protect Management Frame: disable
- Group Key Rotation Interval: 3600

GPIO Schema:

New black PCB's
| MP1: |     |     | MP2: |     |     | MP3: |     |     |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Touch1: | GPIO 12 | *D6* | Touch1: | GPIO 14 | *D5* | Touch1 | GPIO 14 | *D5* |
| ~~Dopplet:~~ | ~~GPIO 12~~ |     | Touch2 | GPIO 13 | *D7* | Touch2 | GPIO 12 | *D6* |
| \-\-\-\-\-\-\-\-\-\- | \-\-\-\-\-\-\-\-\-\- |     | \-\-\-\-\-\-\-\-\-\-\- | \-\-\-\-\-\-\-\-\-\-\- |     | Touch3 | GPIO 13 | *D7* |
| Output 1: | GPIO 5 | *D1* | Output 1 | GPIO 5 | *D1* | Output 1: | GPIO 5 | *D1* |
| \-\-\-\-\-\-\-\-\-\-\- | \-\-\-\-\-\-\-\-\-\-\- |     | Output 2: | GPIO 4 | *D2* | Output 2: | GPIO 4 | *D2* |
| \-\-\-\-\-\-\-\-\-\-\- | \-\-\-\-\-\-\-\-\-\-\- |     | \-\-\-\-\-\-\-\-\-\-\- | \-\-\-\-\-\-\-\-\-\- |     | Output 3: | GPIO 15 | *D8* |
| Speaker | GPIO 15 |     | Speaker | GPIO 0 |     | Speaker | GPIO 0 |     |
| NeoPixel: | GPIO 2 | *D4* | NeoPixel: | GPIO 2 | *D4* | NeoPixel: | GPIO 2 | *D4* |
| Touch Power: | GPIO 16 | *D0* | Touch Power: | GPIO 16 | *D0* | Touch Power: | GPIO 16 | *D0* |


Old green PCB's:
| MP1:    |     || MP2:    |     || MP3:    |     |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Touch1:    | GPIO 13   || Touch1:    | GPIO 12   || Touch1:    | GPIO 14   |
| Dopplet:   | GPIO 12    || Touch2:   | GPIO 13    || Touch2:   | GPIO 12    |
| Output 1:   | GPIO 5    || Output 1:   | GPIO 5    || Touch3:   | GPIO 13    |
| Speaker:    | GPIO 15    || Output 2:    | GPIO 4    || Output 1:   | GPIO 5    |
| RGB Led:   | GPIO 2    || Speaker:   | GPIO 0    || Output 2:   | GPIO 4    |
| Touch Power:   | GPIO 16    || RGB Led:    | GPIO 2    || Output 3:   | GPIO 15    |
|    |     || Touch Power:   | GPIO 16    || Speaker:    | GPIO 0    |
|    |     ||    |     || RGB Led:   | GPIO 2    |
|    |     ||    |     || Touch Power:   | GPIO 16    |
