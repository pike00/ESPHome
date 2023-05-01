# Docker Commands

From [ESPhome.io Guide](https://esphome.io/guides/getting_started_command_line.html#connecting-the-esp-device). ([CLI Reference](https://esphome.io/guides/cli.html))

## Create a new Project
`docker run --rm -v "${PWD}":/config -it ghcr.io/esphome/esphome wizard livingroom.yaml`

## Run
**`Run` uploads and views logs**

`docker run --rm --privileged -v "${PWD}":/config --device=/dev/ttyUSB0 -it ghcr.io/esphome/esphome run livingroom.yaml`

## Upload
**`Upload` only uploads and exits**

`docker run --rm --privileged -v "${PWD}":/config -it ghcr.io/esphome/esphome upload temperature_sensor_1.yaml --device=/dev/ttyUSB0`