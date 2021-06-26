## Connecting and testing the nRF24L01 module
##### To work with the module, you must first enable SPI
To enable SPI, use `raspi-config` or uncomment the` dtparam = spi = on` line in the `/ boot / config.txt` file. Then reboot.
If the SPI driver loads successfully, you will see the device `/ dev / spidev0.0`.
#### Compilation and Build:
`` `sh
$ g ++ -Wall -lrf24 scanner.cpp -o scanner
``,
#### Connection diagram of nRF24L01 + to Raspberry Pi:
! [scheme] (https://github.com/wirekraken/Raspberry-Pi-NRF24/blob/master/scheme/scheme.png)

