# SpaceBall minimal ZMK configuration

Minimal ZMK shield for the SpaceBall PCB using:

- Seeed Studio XIAO nRF52840
- PixArt PMW3610M
- SPI on XIAO D8/D10
- Chip select on XIAO D6
- Interrupt on XIAO D0

Pin mapping:

| PMW3610M | XIAO | nRF52840 GPIO |
|---|---|---|
| IRQ | D0 | P0.02 |
| NCS | D6 | P1.11 |
| SCLK | D8 | P1.13 |
| SDIO | D10 | P1.15 |

The configuration deliberately removes the keyboard matrix, physical layout,
EC11 encoder, split-battery logic, and roBa-specific layers from the original
roBa configuration.

The PMW3610 driver is fetched from:
https://github.com/kumamuk-git/zmk-pmw3610-driver
