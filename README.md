![Blinky Render](/images/Blinky_for_CERBERUS_2100_rev1.jpg)

## Blinky for CERBERUS 2100
Simple board to plug into a [CERBERUS 2100](https://www.thebyteattic.com/p/cerberus-2100.html) and display blinky patterns. It uses a transparent latch (74HVC573) to display the 8-bit data bus on individual LEDs. You can select between the `XCLK` or `XSLC` to drive the display.

The idea is that `XCLK` would continously update with whatever values are on the data bus. Using `XSLC` should only update after a write occurs (but the timing might be off?).


## Future ideas
I may implement a version with a PLD to experiement with programmable logic. 


## Status
Sent rev 1 to the fab. I realize after that I did not provide an easy way to enable the `XE` signal, which turns on the buffers on the CERBERUS 2100. However, there are pads to bodge it.