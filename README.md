# About

-   This image contains the meetecho janus webrtc gateway  ([https://github.com/meetecho/janus-gateway](https://github.com/meetecho/janus-gateway))

-   It uses the google stun server

-   This repository is published here: 
## Limitations

Disables RabbitMQ and MQTT

## Build

`docker build -t vmintam/janus .`

## Ports

| Port   | Description   |
|--------|---------------|
| 80     | HTML-Examples |
| 8088   | RESTful API   |
| 8188   | WebSocket API |

## Environment variables

No environment variables are needed for this image.

## Linked Containers

This container does not need any container linked to.

## Run

`docker run -d -p 7088:7088 -p 8088:8088 -p 8188:8188 -p 8089:8089 -p 8189:8189 -p 61001-62000:61001-62000/udp vmintam/janus:latest`
