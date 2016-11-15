# Run Sonar Qube

## Requirements
* Docker Engine > 1.9
* Docker Compose > 1.6

Use [docker-compose](https://github.com/docker/compose) to start the containers.

```bash
$ docker-compose up
```

You can now access to sonar-server by opening your browser to
```bash
http://127.0.0.1:9000/
```

Restart the containers (after plugin upgrade or install for example).

```bash
$ docker-compose restart sonarqube
```