# A mtc21 Semi-Decoder

A board with all low-level hardware needed to make a Seeed XIAO board a mtc21 decoder.

![Alt text](images/xDuinoRails-Thor-M-3D_Top.png)

## Wiring

```
                     +--------------------+      +--------------------+         +---------------+
                     |      RP2040        |      |     BDR-6133       |         |     Motor     |
                     |    (Top View)      |      |    Motor Driver    |         | DC brushed    |
                     +--------------------+      +--------------------+         +---------------+
                     |                5v  |      |                    |         |               |
          ---``|<----| D15 (LED)      GND |      |                    |         |               |
          ---``|<----| D16 (LED)      3v3 |      |                    |         |               |
                     |                    |      |                    |         |               |
                     |        (PWM B) D8  |----->| InB           OutB |=====+==>| B             |
                     |        (PWM A) D7  |----->| InA           OutA |==+==|==>| A             |
                     |                    |      +---------+----------+  |  |   +---------------+
                     |       (Shut)   A2  |<.............../             |  |
                     |       (bEMF B) A1  |<----------------------------/   |
                     |       (bEMF A) A0  |<-------------------------------/
                     |                    |
                     |                    |      +--------------------+
                     |                    |      | Functions          |
                     |                    |      +--------------------+
                     |         F0f    D9  |----->| F0f                |
                     |         F0b    D10 |----->| F0b                |
                     |                    |      +---------+----------+
                     |       (Shut)   A3  |<.............../

                     |                    |      +--------------------+
                     |                    |      | DCC / Railcom      |
                     |                    |      +--------------------+
                     |     DCC-ACK    D4  |----->| DCC-ACK            |
                     |     DCC/MM/SX  D5  |<-----| DCC/MM/SX          |
                     |     RailCom    D6  |----->| RailCom            |
                     |                    |      +---------+----------+
                     |       (Shut)   A3  |<.............../
                     +--------------------+
```

## Purchase your copy

If you want an easy way to try this board, order one on tindie:
- https://www.tindie.com/products/chatelao/diy-dccmm-decoder-for-xiao-boards
