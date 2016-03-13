# Dangling Volumes

List:
```bash
$ docker volume ls -qf dangling=true
```

Delete:
```bash
$ docker volume rm $(docker volume ls -qf dangling=true)
```
