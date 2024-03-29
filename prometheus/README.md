# Prometheus
##
# Install
Installing prometheus services will launch a prometheus container with all services prometheus.

Prometheus Services: 
- Prometheus Server
- Alertmanager
- Node_exporter
 
 We will use Docker Compose to run multi-container applications with the command below:
 ```
docker compose up
 ```
If you want to run services in the background you can pass the `-d` flag(for "detached" mode)
```
docker compose up -d
```

Stops and removes the containers.
```
docker compose down --rmi all
```
Removing volumes docker compose
```
docker compose down -v --rmi all
```
## 
# Prometheus server
The main Prometheus server which scrapes and stores time series data.

Port
| host    | container  |
| :------ | :--------- |
| `9090`  | `9090`     | 

To access prometheus, open the following URL in your browser:
```
http://localhost:9090
```

## 
# Alertmanager
The Alertmanager seds alerts for slack or E-email

Port
| host    | container  |
| :------ | :--------- |
| `9093`  | `9093`     | 

To access alertmanager, open the following URL in your browser:
```
http://localhost:9093
```

## 
# Node_exporter
Prometheus exporter for hardware and OS metrics exposed by *NIX kernels, written in Go with pluggable metric collectors.

Port
|   host   | container |
|----------|-----------|
|  9113    |   9113    | 

To access node_exporter, open the following URL in your browser:
```
http://localhost:9113