# IOT Infrastructure

## Software

- Thingsboard
- IOT Gateway 
- Mosquitto MQTT

Required to setup manually

- [Mosquitto user credentials][m-conf] - Generate using [tool][m-tool]
- [Local network host ip][gw-to-tb] - Line 2 replace with e.g 192.168.1.198 (without quotes)
- [Thingsboards Gateway access_token][gw-to-tb] - Line 7 (without quotes)
- [Local network host ip][gw-to-gw] - Line 4 replace with e.g. "192.168.1.198" (with quotes)
- [Mosquitto user credentials][gw-to-gw] - Replace lines 9-10 with user and password. 

### Setup host
```sh
./setup
```
### Finally, install 
```sh
docker-compose up
```

[m-conf]: <https://github.com/aPoluden/iot-infra/tree/main/mosquitto-conf/passwd>
[m-tool]: <https://mosquitto.org/man/mosquitto_passwd-1.html>
[gw-to-tb]: <https://github.com/aPoluden/iot-infra/tree/main/tb-gateway-conf/tb_gateway.yaml>
[gw-to-gw]: <https://github.com/aPoluden/iot-infra/tree/main/tb-gateway-conf/mqtt.json>
