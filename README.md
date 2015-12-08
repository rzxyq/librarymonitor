# librarymonitor
Interact with Arduino to monitor how many people went in and out of an library. 

For the website:

Created with django 1.8 and bootstrap. To install the web app, all you need to do is installing python3 and django 1.8. 


For the arduino:

Assume the domain name is example.com, the arduino can send data by sending simply sending a GET request to example.com/sensor.

Send example.com/sensor?data=in if the arduino detects people walking into the library.
Send example.com/sensor?data=out if the arduino detects people walking out of the library. 
Visit example.com/sensor/reset for resetting the database.


Example arduino files are included in arduino_library. Use ultrasonic, WebClient to separately test the sensors and connection to the website. The two programs are combined in LibraryMonitor.
