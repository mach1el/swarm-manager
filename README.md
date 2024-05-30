# swarm-portainer
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Traefik](https://img.shields.io/badge/Traefik-%2341BDF5.svg?style=for-the-badge&logo=Traefik&logoColor=white)
![Portainer](https://img.shields.io/badge/Portainer-%230A0FFF.svg?style=for-the-badge&logo=Portainer&logoColor=white)

This stack combined [Traefik](https://traefik.io/) and [Portainer](https://www.portainer.io/) to manage containers and routing traffice to you swarm services

## Generate the password
```
htpasswd -nBC 10 $TRAEFIK_USER
```

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