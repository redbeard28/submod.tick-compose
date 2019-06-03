# TICK Stack config

## Purpose
This docker-compose file is here to give the possibility to be include in a git submodule call to be include in a ansible role.
 * chronograf
 * influxdb
 * kapacitor

## Volume
It use docker driver NFS.

## Variables
Please, provides thoses variables in your playbook

| vars | what ? | exemple |
|:------:|--------|:-------:|
| {{ tick_chronograf_deploy_replica }} | INTEGER: Number of replica       |    2     |
| {{ tick_kapacitor_deploy_replica }} | INTEGER: Number of replica       |    2     |
| {{ tick_influxdb_deploy_replica }} | INTEGER: Number of replica       |    2     |
| {{ tick_chronograf_port }} | INTEGER: TCP Port      |   8888      |
| {{ tick_kapacitor_port }} | INTEGER: TCP Port      |   9092      |
| {{ tick_influxdb_port }} | INTEGER: TCP Port      |   8086      |
| {{ tick_chronograf_data_nfs_path }}      | STRING: provide full nfs path       | /share/swarm/chronograf/data |
| {{ tick_kapacitor_data_nfs_path }}      | STRING: provide full nfs path       | /share/swarm/kapacitor/data |
| {{ tick_influxdb_data_nfs_path }}      | STRING: provide full nfs path       | /share/swarm/influxdb/data |
| {{ tick_kapacitor_config_nfs_path }}      | STRING: provide full nfs path       | /share/swarm/kapacitor/config |
| {{ tick_influxdb_config_nfs_path }}      | STRING: provide full nfs path       | /share/swarm/influxdb/config |
| {{ grafana_config_nfs_path }}      | STRING: provide full nfs path | /share/swarm/grafana/config |
| {{ tick_nfs_server }}      | STRING: provide IP/hostanme | 192.168.0.2 |
| {{ grafana_dashboards_nfs_path }}      | STRING: provide full nfs path | /share/swarm/grafana/dashboards |










## Licence
See [license](license.md)