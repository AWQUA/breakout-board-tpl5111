# breakout-board-tpl5111

The TPL5111 is a power-gating chip, meant to sit between a power source and a piece of circuitry -- for example a microcontroller -- and periodically cycle power on and off. The TPL5111 consumes only tens of nanoamperes while performing this feat, making it more power-conscious than the lowest deep-sleep setting of many microcontrollers, and a great addition to the design of low-power, long-term environmental monitoring devices. 

The duration of the power cycle is a fixed interval controlled by a resistance applied between ground and the chip's DELAY pin, which may be too limiting for some monitoring devices that need highly dynamic sampling intervals. The delay interval can be set to 0 (always on) by shorting the DELAY pin to the positive rail. Best of all, the chip has a pin (DONE) for receiving a signal that the operation your device was awakened to do has completed and power may be safely turned off.

Datasheet: http://www.ti.com/lit/ds/symlink/tpl5111.pdf
