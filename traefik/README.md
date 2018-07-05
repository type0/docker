![](https://traefik.io/traefik.logo.svg)
# build traefik image

```bash
docker build -t traefik .
```

# run traefik container

```bash
docker run -it -v C:$(pwd):C:/etc/traefik -p 8080:8080 -p 8088:80 traefik --docker.endpoint=tcp://172.25.96.1:2375
```