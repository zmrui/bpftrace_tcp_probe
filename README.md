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

## Example output
```
TIME, source:sport, dest:dport,  data_len, Sequence, AckSequence, snd_cwnd, snd_ssthresh, srtt_us, rcv_wnd
14:00:33.506838,192.168.0.1:47172,10.0.0.2:5201,2896,2400176031,781558132,38,26,267805,42496
```
