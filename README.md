# 🖥️ Task 7: Monitor System Resources Using Netdata

## 📌 Objective
The goal of this task is to install and run **Netdata** using Docker, and visualize **real-time system and application performance metrics** through its dashboard.

---

## ⚡ Steps Performed

1. **Started Docker Desktop** on Windows.
2. Pulled and ran the Netdata container with the following command:
   ```bash
   docker run -d --name=netdata -p 19999:19999 --cap-add SYS_PTRACE --security-opt apparmor=unconfined netdata/netdata
   
3. Verified the container was running using:

   docker ps

Accessed the Netdata dashboard at http://localhost:19999.


Explored and analyzed system metrics:

✅ CPU usage (per-core stats, load average)

✅ Memory & swap usage

✅ Disk I/O (read/write activity)

✅ Network traffic (inbound/outbound)

✅ Docker containers resource usage

✅ Alerts and thresholds panel



📸 Dashboard Screenshot

Below is a snapshot of the Netdata dashboard showing live system metrics:

<img width="1918" height="996" alt="Screenshot 2025-08-16 152856" src="https://github.com/user-attachments/assets/59e1a648-0edb-40ae-a88e-f7b4fdc44d17" />



🎯 Key Learnings

Lightweight & Real-Time: Netdata provides instant, interactive monitoring with zero configuration.

Ease of Deployment: A single Docker run command is enough to start full monitoring.

Wide Coverage: Tracks CPU, memory, disk, network, containers, and more.

Built-in Alerts: Comes with pre-configured thresholds for proactive monitoring.

Useful for DevOps: Ideal for debugging performance issues on servers and applications.



✅ Outcome

By completing this task, I gained hands-on experience with monitoring servers and applications using Netdata, explored system health metrics, and understood how lightweight monitoring tools can assist in real-time DevOps operations.
