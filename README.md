## Adafruit TCS3448 14-Channel Light / Color Sensor Breakout - STEMMA QT / Qwiic PCB

<a href="http://www.adafruit.com/products/6525"><img src="assets/6525.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit TCS3448 14-Channel Light / Color Sensor Breakout - STEMMA QT / Qwiic. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/6525

### Description

The <b>Adafruit TCS3448 (a.k.a TCS34488) Multi-Spectral Sensor</b> is a multi-channel spectrometer, which is a special type of light sensor that is able to detect not only the amount of light present but also the amounts of light within different wavelengths. This means that you can use it to detect much better than the human eye is capable of, what color or colors of light is present.

The TCS3448 packs within its 3x2mm footprint 25 photodiodes that can detect 11 separate, overlapping bands of visible light, plus one near infrared, one clear and a flicker channel for 14 channels total. Compared to the AS7341, this sensor has 4 more light channels - but you'll need to use a new firmware driver since it's not back-compatible.

<b>The TCS3448 is ams Osram's 'refresh' of the AS7343</b>, so it's an upgrade from the AS7341 and has some slight improvements/changes over the AS7343: 

* I2C address changed from 0x39 to 0x59.
* Retuned optical filters: channel centers move by a few nanometers and several visible channels have higher responsivity especially violet/blue and the F8 far-red channel.
* Sensitivity is not higher everywhere; NIR response is lower.
* Firmware is not 100% drop-in! You'll need to recompile since the I2C address has changed

The multi-spectral color measuring capabilities of the TCS3448 can be used to quantify the specific makeup of light, either emitted or reflective. It's kind of like a mini spectroscopy sensor. This is possible thanks to the impressive collection of sensors in the TCS3448 being routed through 6 independent 16-bit ADCs that take the raw measurements and convert them to digital values that can be read out over I2C.

14 readable individual sensor elements (13 light channels plus flicker detection) don’t exactly fit through a 6-channel ADC all at once, so the chip includes a so-called Super MUX (SMUX) that allows you to route the signal from any sensor to any ADC channel. The sensor also has GPIO and interrupt pins that can allow it to communicate directly with other sensors, or the microcontroller itself.

All of this capability is made accessible by mounting the sensor on a STEMMA QT form factor breakout board, complete with level shifting circuitry and [SparkFun Qwiic](https://www.sparkfun.com/qwiic) compatible [Stemma QT](https://learn.adafruit.com/introducing-adafruit-stemma-qt) connectors. This means that you can, without needing to solder, connect our TCS3448 breakout into your 3.3V or 5V microcontroller of choice be it an Arduino Uno, Raspberry Pi, or one of the many [CircuitPython-compatible boards](https://circuitpython.org/downloads). While it certainly takes a bit of work to make all those different light sensors share their measurements, our Arduino and CircuitPython libraries take care of all of that hard work for you and even include example code to help get you started. [QT Cable is not included, but we have a variety in the shop](https://www.adafruit.com/?q=stemma+qt+cable&sort=BestMatch).

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
