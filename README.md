# Pynq-Z2-LED
VHDL code to toggle on-board LEDs on PYNQ-Z2 FPGA board. Push button switches control the direction of LED toggling in LEFT and RIGHT directions.

## Structure
Top module: leds_toggle_top.vhd
Sub modules: slow_clock.vhd, push_button.vhd, led_toggle.vhd

<b>slow_clock.vhd:</b> <i> Generates a slow clock of 1Hz from an on-board 125MHz. <i/>
<br />
<b>push_button.vhd:</b> Latches the push button value.
<br />
<b>led_toggle.vhd:</b> Toggles on-board 4-LEDs in LEFT or RIGHT directions set by the on-board push buttons BTN1 and BTN2 respectively
<br />
<b>led_toggle_tb.vhd:</b> Test bench for simulation
<br />

## Simulation
![WaveForm](https://user-images.githubusercontent.com/127403893/224462408-38ab37dd-d556-4b90-98b9-d5bd7e6befdc.JPG)

## LEDs Test
![gif_1678434190289](https://user-images.githubusercontent.com/127403893/224254519-bb5f76c4-de98-47c5-9464-0eb0dd9b3021.gif)
<br />
Fig: LED toggling in LEFT
<br />
<br />
![gif_1678435109398](https://user-images.githubusercontent.com/127403893/224257826-68b08684-5e0f-471a-a691-7ae5fafcc718.gif)
<br />
Fig: LED toggling in RIGHT
<br />
