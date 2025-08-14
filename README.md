1. Run Netdata in Docker

docker run -d \
  --name=netdata \
  -p 19999:19999 \
  --cap-add SYS_PTRACE \
  --security-opt apparmor=unconfined \
  netdata/netdata


2. Open Dashboard

Go to http://localhost:19999 in your browser.

You’ll see CPU, memory, disk, network, and Docker metrics updating in real-time.

3. Explore Metrics

Scroll through charts.

Look at Docker containers tab if you have any running.

Check alerts and panel descriptions.
