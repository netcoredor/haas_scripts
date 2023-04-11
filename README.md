# haas_scripts
The latest RadonEye RD200 is not supported out of the Haas box, so I came up with this workaround to read the values.
Random Yaml files for Home Assistant

Step 1. Change your service_uuid and characteristic_uuid to match your device.

service_uuid: "00001523-0000-1000-8000-00805F9B34FB"
characteristic_uuid: "00001524-0000-1000-8000-00805F9B34FB"
Note: you can retrieve these using many different mobile phone blutooth monitoring applications.

Step 2. After flashing the ESP32 that will communicate with your RadonEye, configure the new esp32 sensor to switch 'on' every X seconds in order to trigger the read value and notify.
