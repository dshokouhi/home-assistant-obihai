# home-assistant-obihai
obihai sensor for home-assistant

Currently tested on obi110. To install, put the `__init__.py` and `sensor.py` under
<config_dir>/custom_components/obihai/


in the configuration.yaml add
```
sensor:
  - platform: obihai
    host: <IP of obihai>
    password: <password>
```
