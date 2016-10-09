# Mainflux Gateway

### About
Mainflux Gateway is a gateway firmware application that connects a subnet behind an MQTT gateway to the central Mainflux server.

### Install/Deploy

Install Paho MQTT Lua package:
```bash
git clone https://git.eclipse.org/r/paho/org.eclipse.paho.mqtt.lua
cd org.eclipse.paho.mqtt.lua/
luarocks make rocks/paho-mqtt-0.3.0-1.rockspec
```

Run it:
```bash
lua mainfluxGateway.lua -t mainflux/main
```

Send some messages to it:
```bash
mosquitto_pub -t mainflux/main -m "123"
```

### Documentation
Development documentation can be found on our [Mainflux GitHub Wiki](https://github.com/Mainflux/mainflux/wiki).

### Community
#### Mailing list
[mainflux](https://groups.google.com/forum/#!forum/mainflux) Google group

For quick questions and suggestions you can also use GitHub Issues.

#### IRC
[Mainflux Gitter](https://gitter.im/Mainflux/mainflux?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

#### Twitter
[@mainflux](https://twitter.com/mainflux)

### Authors
Main architect and BDFL of Mainflux project is [@drasko](https://github.com/drasko).

Maintainers are listed in [MAINTAINERS](MAINTAINERS) file.

### License
[Apache License, version 2.0](LICENSE)
