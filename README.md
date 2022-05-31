# temporary_libmdns_fix_for_arduino-esp32
This is here just temporarily, I will remove this once it's been properly fixed :)

## For users of PlatformIO on Windows :
Go to:
```
C:\Users\<Your UserName>\.platformio\packages\framework-arduinoespressif32
```
and drag and drop the tools folder from this repository this should replace all mdns related files.

If it doesn't work you might have to manually specify arduino-esp32 2.0.3 in ```platformio.ini``` in your project like so:
```
platform_packages = 
    framework-arduinoespressif32@https://github.com/espressif/arduino-esp32.git#2.0.3    
```
If you do this the path slightly changes and something with @ is added to the end you have to look for this yourself though because I'm not sure if it's the same for everyone:
```
C:\Users\<Your UserName>\.platformio\packages\framework-arduinoespressif32@src-etcetc
```
and drag and drop the tools folder from this repo in there.

## For users of the Arduino IDE on Windows (I didn't test this out, just adding it here):
Go to:
```
C:\Users\<Your UserName>\AppData\Local\Arduino15\packages\esp32\hardware\esp32\2.0.3
```
drag and drop the tools folder from this repository this should replace all mdns related files.



### Make sure it's the latest version 2.0.3 and 
#### Hope this Helps :)
