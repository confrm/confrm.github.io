---
title: USB Switch Design
tags: IOT, esp8266, usb\_switch
---

JLC have delivered and everything fits perfectly:

![USB Switch PCB](/assets/images/2021-02-12-1.jpg)

Looking good, have done a few revisions of the case. Currently the case is modelled in On-Shape, which is convenient but not great for sharing - so need to move the design to FreeCAD.

In related news the ESP8266 support in confrm is working, which now opens up the ability to integrate with Tasmota.

I have also been looking at some changes to the overall design to push the price down. USB2 gives a significant saving, and using a MOSFET in place of the relay is an option. The MOSFET will waste some power and generate a little bit of heat.

Parts are on order for some testing.
