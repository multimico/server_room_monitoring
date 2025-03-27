# Server Room Monitoring

This repository provides a guide for setting up a graphical monitoring system to track the temperature and humidity of a server room. The solution involves collecting data from a Temperatur/Humidity sensor connected to a Raspberry Pi 3b, storing it in a database, and visualizing it using a Grafana dashboard.
Overview

The repository includes a docker-compose.yml file that sets up three containers:

InfluxDB: A time-series database that stores the collected metrics.
Grafana: A visualization tool that displays the data in a customizable dashboard.
Caddy: A reverse proxy that exposes the Grafana dashboard securely via a web browser.


## Usage

To build and run the containers, execute the following command:
```bash

docker-compose up -d
```

Once deployed, you can access the Grafana dashboard through your web browser via the configured Caddy reverse proxy.
