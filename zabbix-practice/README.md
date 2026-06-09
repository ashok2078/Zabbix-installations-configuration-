# DevOps Project: Infrastructure Monitoring with Zabbix

This repository contains the complete setup, configuration, and troubleshooting documentation for an Enterprise Infrastructure Monitoring Lab using Docker Containers on a CentOS/Linux environment.

---

##  Project Architecture
The architecture is fully containerized using Docker and consists of the following components:
* **Zabbix Server & Web Interface:** Core monitoring engine and dashboard.

* **Zabbix Agent 2:** Deployed on a target Linux server to collect system metrics.


---

##  Deployment & Operations Commands

### 1. Initialize and Start Containers
bash
#docker-compose up -d

*** Enable Auto-Start Policy ***
#docker update --restart always zabbix-db zabbix-server zabbix-web target-server-agent

(Configures the Docker daemon to automatically restart the Zabbix infrastructure containers if the main Linux host system reboots or crashes.)

*** Check Live Container Status ***
#docker ps
(Lists all currently active and running Docker containers along with their status, uptime, and exposed network ports.)
<img width="1330" height="678" alt="image" src="https://github.com/user-attachments/assets/1a479590-2fa8-46f2-a4d6-464a0e1d518d" />



