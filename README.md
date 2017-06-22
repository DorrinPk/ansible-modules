## Collectd module for metrics

This Collectd module gathers metrics and sends them to an influxdb instance located on `10.0.1.227`.

currently it tracks the systems :

* battery
* cpu
* disk
* memory
* network
* swap
* uptime
* users

If you'd want to add more module, configure them in `/files/collectd.conf (for ubuntu) and collectdyum.conf for RHEL`
to run the collectd module, fill up the tmp file with the ip addrs of your desired hosts and run:

`ansible-playbook -i ansible/tmp  ansible/collectd/tasks/main.yml -K`

### ANSIBLE VERSION 2.0.0 AND HIGHER REQUIRED

influxdb interface : http://10.0.1.227:8083/
grafana interface : http://10.0.1.227:3000/
