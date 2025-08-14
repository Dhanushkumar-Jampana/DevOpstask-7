# Task 7 - Monitor System Resources Using Netdata

## Objective
Install and run Netdata to visualize real-time system and application performance metrics.

## Steps Followed
1. Pulled and ran Netdata using Docker:
   ```bash
   docker run -d \
     --name=netdata \
     -p 19999:19999 \
     --cap-add SYS_PTRACE \
     --security-opt apparmor=unconfined \
     netdata/netdata
2.Accessed the Netdata dashboard at:

http://localhost:19999

3.Monitored:

CPU usage

Memory usage

Disk read/write

Docker container metrics
