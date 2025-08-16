# Netdata-Monitoring
Monitor System Resources Using Netdata (DevOps Internship Task)

Monitor System Resources Using Netdata

## Objective
Install and run **Netdata** using Docker to monitor system and application performance in real-time.

## Steps
1. Started Docker Desktop on Windows.
2. Ran Netdata container:
   ```bash
   docker run -d --name=netdata -p 19999:19999 --cap-add SYS_PTRACE --security-opt apparmor=unconfined netdata/netdata
