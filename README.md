# simple-heart-rate-monitoring


This is simple project based on IoT device

Arduino is the basic platform this project works on. ESP8266 Wi-Fi module takes analog values from the Pulse Sensor and upload the data into ThingSpeak server over Internet with a small battery connected to it as a power source. The Pulse Sensor detects the Beats per Minute (BPM) of a person. The circuit is wired up with a 4.7K Ohm Resistor, 10K Ohm Resistor and a 10 micro Farad Capacitor. Resistors are used for voltage regulations and capacitor is used to reduce the voltage buffer, so that noise from Pulse Sensor can be reduced when ESP8266 collects the analog data.

The recorded data of sensors is saved in thingspeak server which is platform for IoT devices, The sensor data is sent through the inbuilt ESP8266 wifi in NODEMCU while we connect it to our private wifi.

This data can also be seen in our mobile by installing pocket IoT application from play store, in this application we have to input our channel ID and write API key which can be available in thingspeak server of our channel.

NOTE: We can use any of the device Arduino uno or NODE MCU which is nothing but a arduino device with a built in wifi, i have use NODE MCU because there are some kernel and compatability issues with ESP8266 wifi module when plugged in with Arduino uno board.



PROCESS:

First of all, user needs to Create a Account on ThingSpeak.com, then Sign In and click on Get Started.

Now go to the ‘Channels’ menu and click on New Channel option on the same page for further process.

Now you will see a form for creating the channel, fill in the Name and Description as per your choice. 

Then fill ‘Pulse Rate’ in Field label, tick the checkboxes for the Fields.

Also tick the check box for ‘Make Public’ option below in the form and finally Save the Channel. 

Now your new channel has been created.

You will see a chart. Note the Write API key, we will use this key in our code.

![image](https://user-images.githubusercontent.com/56999611/119227753-1aa6e600-bb2d-11eb-8c8e-24d7a12b9035.png)

then connect the circuit as shown in the above image 
connect it to the pc where you run the code,code should be run on arduino compiler which can be downlaoded from https://www.arduino.cc/en/software from this website
once you connect the device to the pc and open the IDE then update all the kernels to your Iot device by selecting the port which it is connected to
RUN the CODE...

if you want to monitor it on the smartphone then download pocket IOT app from playstore,copy the channel ID and API key from thingsspeak channel that we created earlier, paste it there and you can see the graph and your results.

