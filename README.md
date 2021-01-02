# Obihai custom component
Obihai sensor for Home Assistant - All code current with release 2020.12

Currently tested on obi110 and obi200. To install, place `__init__.py` `manifest.json` and `sensor.py` under:

`<config_dir>/custom_components/obihai/`


in the configuration.yaml add
```
sensor:
  - platform: obihai
    host: <IP of obihai>
    password: <password>
```
note if using the user account you need to add `username: user` to the configuration.

`sensor.obihai_port_status` will be either `On Hook` `Off Hook` or `Ringing` (maybe something else too)

The other sensors will be `0` if no active calls and `1` if there is an active call (number may be higher if you have more lines on the same SP line)
