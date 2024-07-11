# Bpftrace TCP Probe

## Background

https://lore.kernel.org/lkml/151374331148.2497.8420025110359616202.stgit@devbox/


## Attention
This script tracing __ip_local_out function and will output every IP packet send out message in terminal. This is writen for research purposed.

## Steps

Install bpftrace
https://github.com/bpftrace/bpftrace

In one terminal
``` shell
sudo ./ip_local_out.bt
```

In another terminal
```shell
curl google.com
```
