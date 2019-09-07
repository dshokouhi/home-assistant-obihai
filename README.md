# home-assistant-obihai
Obihai sensor for home-assistant

Currently tested on obi110 and obi200. To install, place `__init__.py` and `sensor.py` files under:

`<config_dir>/custom_components/obihai/`


in the configuration.yaml add
```
sensor:
  - platform: obihai
    host: <IP of obihai>
    password: <password>
```

`sensor.port_status` will be either `On Hook` `Off Hook` or `Ringing` (maybe something else too)

The other sensors will be `0` if no active calls and `1` if there is an active call (number may be higher if you have more lines on the same SP line)
