This API automatically retrieves the list of available V4L2 controls. There's a function to retrieve the list of controls and thus know the driver's capabilities, and there are also control getter and setter functions using either the control name, for example "exposure", or using the control ID "0xFFFFFFF". This allows the exposure time to be controlled either by its name or by its ID, depending on the developer's choice.
The API also allows the sensor to be launched in different sensor_modes. For example, sensor_mode 2 corresponds to the GRAY8 format in 1080p.

# Dependecy 

- libv4l-dev

# Installation

 ```gcc -shared -o topaz_api.so -fPIC topaz_api.c ```

 ```sudo mv topaz_api.so /usr/local/lib/```

 ```sudo cp topaz_api.h /usr/local/include/```
