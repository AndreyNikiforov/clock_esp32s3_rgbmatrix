# Desk Clock with RGB Matrix

# Development

## Building

```shell
cargo build
```

## Flashing

### Web flash

```shell
scripts/flash.sh debug
```

### Remote Serial port

Cannot flash from within dev container (seems that MacOS do not pass serial ports to docker): need flash web server running on the host or serial-over-tcp proxy

#### RFC2217

#### Raw Serial

[doc](https://docs.espressif.com/projects/esptool/en/latest/esp32/esptool/remote-serial-ports.html)
[macos issues with stty for speed setting](https://discussions.apple.com/thread/3798003?tstart=0&sortBy=rank) and [FreeBSD workaround](https://www.clearchain.com/blog/posts/using-serial-devices-in-freebsd-how-to-set-a-terminal-baud-rate)

## Simulator

[Matrix](https://www.arduinolibraries.info/libraries/esp32-hub75-led-matrix-panel-dma-display)

# Ad Hoc links

[Using DMA for RGB Matrix](https://github.com/mrcodetastic/ESP32-HUB75-MatrixPanel-DMA)
[HUB75 support in embedded-graphics](https://github.com/david-sawatzke/hub75-rs)
[BCM](https://www.batsocks.co.uk/readme/art_bcm_4.htm)