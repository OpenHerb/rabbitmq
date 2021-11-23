# OpenHerb MQTT Broker

![img](docs/img/icon.png)

Modified: 2021-11
## Usage
`OpenHerb/rabbitmq` extends the RabbitMQ management broker including custom initialization declarations and plugins. he image is packaged for arm64 and x86 systems, simply reference using the `arm64` or `x86` tags. From github container registry:
```bash
docker pull ghcr.io/openherb/rabbitmq:arm64
```
Or for x86 architectures:
```bash
docker pull ghcr.io/openherb/rabbitmq:x86
```

Or integrate the container in any compose stack:
```yaml
services:
  rmq:
    container_name: rmq
    image: ghcr.io/openherb/rabbitmq:arm64
	restart: always
    ports:
      # expose for rmq management client
      - "15672:15672"
    networks:
      - mqtt
```
