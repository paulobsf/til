# TCP Dump

Dump traffic on a network.

Capture traffic to / from a host:

```bash
&#35; tcpdump host {{www.example.com}}
```


Capture traffic in interface to port, include data, don't convert address to names:

```bash
&#35; sudo tcpdump -vvXni <interface> 'dst port <port>'
```
