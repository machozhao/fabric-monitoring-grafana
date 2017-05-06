# fabric-monitoring-grafana
Monitoring Hyperledge Fabric docker via (cAdvisor + InfluxDB + Grafana) Stack

## Access and setup Grafana
### Login Grafana
```
http://localhost:3000
login with default user: admin/admin
```
!["Login Grafana"](https://github.com/machozhao/fabric-monitoring-grafana/raw/master/docs/images/p1.grafana.login.png)
*Fig. 1: Login Grafana*

### Add Data source
```
Data source name: influxdb
Data source type: InfluxDB
Http settings url: http:/influxsrv:8086
Http Auth: Basic Auth
Basic Auth Detail: admin/admin
InfluxDB details: database: cadvisor, user: root, password: root
```
!["Add data source"](https://github.com/machozhao/fabric-monitoring-grafana/raw/master/docs/images/p2.grafana_add_data_source.png)
*Fig. 2: Add data source*

### Import a Dashboard
```
Import databoard json file: grafana-dashboard/docker-monitoring.json
```
!["Import a dashboard"](https://github.com/machozhao/fabric-monitoring-grafana/raw/master/docs/images/p3.grafana.import.dashboard.png)
*Fig. 3: Import a dashboard*

### Access dashboard
!["Import a dashboard"](https://github.com/machozhao/fabric-monitoring-grafana/raw/master/docs/images/p4.grafana.dashboard.png)
*Fig. 4: Access dashboard*
