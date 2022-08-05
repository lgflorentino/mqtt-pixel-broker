MQTT-Example-Broker
===

# Description

A quick app using cpp to demo for the pixel badge
Needs the [mqtt_cpp](https://github.com/redboltz/mqtt_cpp) header at `/opt/share/mqtt_cpp`

Uses [meson](https://mesonbuild.com) for the build system

# To build
```zsh
meson setup builddir

(cd builddir && ninja)

```



