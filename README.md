# simple-heart-rate-monitoring

This is simple project based on IoT device

Arduino is the basic platform this project works on. ESP8266 Wi-Fi module takes analog values from the Pulse Sensor and upload the data into ThingSpeak server over Internet with a small battery connected to it as a power source. The Pulse Sensor detects the Beats per Minute (BPM) of a person. The circuit is wired up with a 4.7K Ohm Resistor, 10K Ohm Resistor and a 10 micro Farad Capacitor. Resistors are used for voltage regulations and capacitor is used to reduce the voltage buffer, so that noise from Pulse Sensor can be reduced when ESP8266 collects the analog data.
 

The recorded data of sensors is saved in thingspeak server which is platform for IoT devices,
The sensor data is sent through the inbuilt ESP8266 wifi in NODEMCU while we connect it to
our private wifi.

This data can also be seen in our mobile by installing pocket IoT application from play store,
in this application we have to input our channel ID and write API key which can be available
in thingspeak server of our channel.

NOTE: We can use any of the device Arduino uno or NODE MCU which is nothing but a arduino device with a built in wifi, i have use NODE MCU because there are some kernel and compatability issues with ESP8266 wifi module when plugged in with Arduino uno board.





