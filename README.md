# Zabbix Monitoring Stack in Docker

## Project Description

This project provides a Docker Compose setup for deploying a complete Zabbix Monitoring Stack, including:

- **Zabbix Server**: Core server component that collects and processes monitoring data.
- **Zabbix Web Interface**: User-friendly web interface for configuring, viewing, and managing Zabbix data.
- **PostgreSQL**: Database for storing Zabbix data.
- **Zabbix Agent**: Configured to monitor the host system metrics through Docker API integration, simulating an agent installed directly on the host.

## Components

- **PostgreSQL**: Database for Zabbix, storing monitoring data.
- **Zabbix Server**: The main server that gathers and processes all monitoring data.
- **Zabbix Web Interface**: Web-based interface for managing and viewing Zabbix data.
- **Zabbix Agent**: Configured within a container to access and monitor host system metrics, acting as a local agent.

## Features

- **Docker-Ready Configuration**: All services and network configuration are defined in a single `docker-compose.yml` file.
- **Optional SSL**: Allows for secure connections if configured.
- **Host-Level Monitoring**: Zabbix Agent is configured to connect to the Docker API, allowing it to gather host OS metrics directly from the containerized environment.

## Setup

1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd zabbix-monitoring-stack
