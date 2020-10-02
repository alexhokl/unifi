# unifi

Docker image of Unifi controller

## Run

### Version 6

```sh
docker-compose up -d
```

### Version 5

```sh
docker run -d --restart always -v /etc/localtime:/etc/localtime:ro --name unifi -v $HOME/unifi-config:/config -p 3478:3478/udp -p 10001:10001/udp -p 8080:8080 -p 8081:8081 -p 8443:8443 -p 8843:8843 -p 8880:8880 alexhokl/unifi:5.12.66
```

## References

- [jessfraz/dockerfiles](https://github.com/jessfraz/dockerfiles/tree/master/unifi)
- [jacobalberty/unifi-docker](https://github.com/jacobalberty/unifi-docker)
