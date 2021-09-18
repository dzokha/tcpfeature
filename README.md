# Tcpfeature

Tcpfeature module is proposed to extract, normalize 29 features from network packets

Please cite the paper if it can help you. Thank you very much.

```
V. K. Nguyen, M. Nhat Quang Truong, V. L. Le, Q. Thang Le and T. H. Nguyen, "A Novel Approach for Data Collection and Network Attack Warning," 2019 11th International Conference on Knowledge and Systems Engineering (KSE), 2019, pp. 1-6, doi: 10.1109/KSE.2019.8919494.
```


# 29 characteristics of network attack data

| # | Feature | Description |
|---|---------|-------------|
| 1 | duration | length (number of seconds) of the connection |
| 2 | protocol_type | type of the protocol, e.g. tcp, udp, etc. |
| 3 | service | network service on the destination, e.g., http, telnet, etc. |
| 4 | flags | normal or error status of the connection |
| 5 | src_bytes | number of data bytes from source to destination |
| 6 | dst_bytes | number of data bytes from destination to source |
| 7 | land | 1 if connection is from/to the same host/port; 0 otherwise |
| 8 | wrong_fragment | number of "wrong'' fragments |
| 9 | urgent | number of urgent packets |
| 10 | hot | number of 'hot' indicators (bro-ids feature) |
| 11 | count | number of connections to the same host as the current connection in the past two seconds |
| 12 | srv_count | number of connections to the same service as the current connection in the past two seconds |
| 13 | serror_rate | % of connections that have "SYN'' errors (same-host) |
| 14 | srv_serror_rate | % of connections that have "SYN'' errors (same-service) |
| 15 | rerror_rate | % of connections that have "REJ'' errors (same-host) |
| 16 | srv_rerror_rate | % of connections that have "REJ'' errors (same-service) |
| 17 | same_srv_rate | % of connections to the same service (same-host) |
| 18 | diff_srv_rate | % of connections to different services (same-host) |
| 19 | srv_diff_host_rate | % of connections to different hosts (same-service) |
| 20 | dst_host_count | count of connections having the same destination host |
| 21 | dst_host_srv_count | count of connections having the same destination host and using the same service | 
| 22 | dst_host_same_srv_rate | % of connections having the same destination host and using the same service | 
| 23 | dst_host_diff_srv_rate | % of different services on the current host |
| 24 | dst_host_same_src_port_rate | % of connections to the current host having the same src port | 
| 25 | dst_host_srv_diff_host_rate | % of connections to the same service coming from different hosts |
| 26 | dst_host_serror_rate | % of connections to the current host that have an S0 error |
| 27 | dst_host_srv_serror_rate | % of connections to the current host and specified service that have an S0 error |
| 28 | dst_host_rerror_rate | % of connections to the current host that have an RST error |
| 29 | dst_host_srv_rerror_rate | % of connections to the current host and specified service that have an RST error |

# References

1. http://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html
2. https://www.ll.mit.edu/r-d/datasets/1999-darpa-intrusion-detection-evaluation-dataset
