# Compressing a directory into multiple files

Zip recursively with "split-size" in MB:

```bash
$ zip -r -s archive.zip dir_name/
```

Results in (example):

```
archive.z01 archive.z02 archive.z03 archive.z04 archive.z05 archive.zip
```
