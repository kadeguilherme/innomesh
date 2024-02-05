# Prometheus
##
# Install
Installing prometheus services will launch a prometheus container with all services prometheus.

Prometheus Services: 
- Prometheus Server
- Alertmanager
- Node_exporter
 
 You launch container with command bellow
 ```
docker compose up
 ```
If you want to run services in the background you can pass the `-d` flag(for "detached" mode)
```
docker compose up -d
```

Stop your prometheus
```
docker compose stop
```
Remove `--volumes`
```
docker compose down --volumes
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
