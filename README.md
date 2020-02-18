KiCAD Board Files for an open source adapter that allows hacking and protyping 
with GE appliances.

### Note: these haven't been tested or produced.

They are based off of GE's official implementation. I've reverse engineered an 
interface on an oven board, and this is essentially a half-duplex to full-duplex 
UART converter. It can talk to two appliances at once, as it has two channels.
A smaller, single channel variant is in the works.

#### RJ45 port pinout:
1. GND
2. GEA_E (half-duplex 19200 baud)
3. 9-14VDC
4. GEA2_RXD (full-duplex 230400 baud)
5. GEA2_TXD
6. 5V
7. NC
8. NC
