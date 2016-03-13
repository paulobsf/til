# Inspect IP address

Inspect the IP address of a running container (uses [jq](https://stedolan.github.io/jq/)):

```bash
$ docker inspect mysql-tests | jq '.[0] | .NetworkSettings.IPAddress'
```
