# swarm-portainer
This stack combined [Traefik](https://traefik.io/) and [Portainer](https://www.portainer.io/) to manage containers and routing traffice to you swarm services

## Run
```
docker stack deploy -c stack.yml manager
```

## Variables

| Name | Description | Default |
|------|-------------|---------|
|<a name="DOMAIN"></a> [DOMAIN](#) | Set DNS for cotainers resource | `traefik.me` |
|<a name="TRAEFIK_USER"></a> [TRAEFIK_USER](#) | User for traefik middlewares authentication  | `admin` |
|<a name="TRAEFIK_PASSWD"></a> [TRAEFIK_PASSWORD](#) | Password for traefik middlewares authentication  | `traefik@admin` |