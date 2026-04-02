This repository constaints POC implementation.
For actively maintained version see one of fork, eg [tostmann/esp-coordinator](https://github.com/tostmann/esp-coordinator).

ZBOSS NCP Serial Protocol implementation for ESP32-C6/H2 module.

This implementation functional limited to coordinator role for usage with [zigbee2mqtt](https://www.zigbee2mqtt.io).

[Protocol specification](https://wiki.homed.dev/files/9/95/ZBOSS_NCP_Serial_Protocol.pdf)

Configuration examle:
```
serial:
  port: /dev/cu.usbmodem1101
  adapter: zboss
```

At [releases](https://github.com/andryblack/esp-coordinator/releases) example firmware build for [WeAct Studio ESP32-C6-mini module](https://aliexpress.ru/item/1005006800070921.html)

Flashing offsets:
```
0x0 bootloader.bin
0x20000 esp-coordinator.bin
0x8000 partition-table.bin
0xf000 ota_data_initial.bin
```
