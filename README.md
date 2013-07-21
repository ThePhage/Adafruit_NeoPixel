Adafruit NeoPixel library
=========================

Phage modifications:
 - added API calls to enable length detection. in particular, had to modify the number of pixels in a strand to be a dynamic parameter, and also had to dup the pin toggling code into a separate call that follows it up with a rapid set of input port reads. A looped back strand will create a single pulse that is detectable by the microcontroller (in this case an ATTiny85). At the moment, the paramenters are hard-coded for use with just the phage-armband application.

=========================

Arduino library for controlling single-wire-based LED pixels and strip such as the [Adafruit 60 LED/meter Digital LED strip][strip], the [Adafruit FLORA RGB Smart Pixel][flora], the [Adafruit Breadboard-friendly RGB Smart Pixel][pixel], the [Adafruit NeoPixel Stick][stick], and the [Adafruit NeoPixel Shield][shield].

After downloading, rename folder to 'Adafruit_NeoPixel' and install in Arduino Libraries folder. Restart Arduino IDE, then open File->Sketchbook->Library->Adafruit_NeoPixel->strandtest sketch.

[flora]:  http://adafruit.com/products/1060
[strip]:  http://adafruit.com/products/1138
[pixel]:  http://adafruit.com/products/1312
[stick]:  http://adafruit.com/products/1426
[shield]: http://adafruit.com/products/1430
