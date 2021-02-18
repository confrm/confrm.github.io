# Welcome to confrm.io

Confrm is a provisioning tool for IOT devices. Created to provide an easy way to update things which are embedded in walls, stuck in hard to reach boxes and halfway up the garden, it also provides a convenient mechanism to monitor those devices and configure them remotely.

Most IOT devices will already have wifi stacks and http libraries, Confrm uses a basic REST API to enable those device to query a central server for updates / configuration information.

Eventually we want to add more features and integrations in to larger projects - but for now we just support esp32/esp8266 devices using Arduino / platform.io.

See [https://github.com/confrm/confrm](https://github.com/confrm/confrm) for the server and the following repositories for the device code:

* confrm-arduino-esp (ESP32, ESP8266) [https://github.com/confrm/confrm-arduino-esp](https://github.com/confrm/confrm-arduino-esp)

