# unifi

Docker image of Unifi controller

## Run

```sh
docker run -d --restart always -v /etc/localtime:/etc/localtime:ro --name unifi -v $HOME/unifi-config:/config -p 3478:3478/udp -p 10001:10001/udp -p 8080:8080 -p 8081:8081 -p 8443:8443 -p 8843:8843 -p 8880:8880 alexhokl/unifi:latest
```
