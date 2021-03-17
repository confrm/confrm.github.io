# Adding Confrm to Applications

## Arduino IDE

There are three ways to add Confrm to the Arduino IDE; via the library manager, using a zip file or adding the files manually to the project. This article at maker.io covers the steps required for all three:

[https://www.digikey.co.uk/en/maker/blogs/2018/how-to-install-arduino-libraries](https://www.digikey.co.uk/en/maker/blogs/2018/how-to-install-arduino-libraries)

The github repository for ESP32 and ESP8266 devices is [https://github.com/confrm/confrm-arduino-esp](https://github.com/confrm/confrm-arduino-esp).

## Platformio

Using platformio "confrm" can be added to the lib\_deps in platform.ini:

``` ini
lib_deps = 
  other-library@2.1
  confrm
```

Or the git repository can be added directly using:

``` ini
lib_deps_external =
  https://github.com/confrm/confrm-arduino-esp.git#main
```

In this instance using the main branch, but it could be any specific verison tag or branch.

## Demonstration

And this video covers how to write a simple esp32 program which will register with the confrm server as a programmable node:

<iframe width="560" height="315" src="https://www.youtube.com/embed/tlPyaRXVDFw" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

