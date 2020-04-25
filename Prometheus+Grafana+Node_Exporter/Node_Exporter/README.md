#The Prometheus Node Exporter exposes a wide variety of hardware- and kernel-related metrics.


In this guide, you will:
  *Start up a Node Exporter on localhost
  *Start up a Prometheus instance on localhost that's configured to scrape metrics from the running Node Exporter

Documentations
==============

https://www.fosslinux.com/10398/how-to-install-and-configure-prometheus-on-centos-7.htm

<img width="750" alt="Screenshot_541" src="https://user-images.githubusercontent.com/13994900/80279349-bc59ca80-86c2-11ea-9df8-7f4dd1084ef2.png">

Prerequistes
==============

* yum install ansible wget git 
* Python Version - Python 2.7.5 

Steps
======
1. git clone 
2. cd cd ansible-playbooks-tatiana/Prometheus+Grafana+Node_Exporter/Node_Exporter/
3. ansible-playbook node_exporter.yaml
4. systemctl status node_exporter
<img width="650" alt="Screenshot_544" src="https://user-images.githubusercontent.com/13994900/80281443-d1d5f100-86d0-11ea-9926-90499f39f01f.png">
5. http://Server-IP:9100
<img width="650" alt="Screenshot_545" src="https://user-images.githubusercontent.com/13994900/80281492-24171200-86d1-11ea-9b14-d69653edd1af.png">

