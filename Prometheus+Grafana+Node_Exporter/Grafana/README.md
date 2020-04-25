What is Grafana?
=================

* Grafana is open source visualization and analytics software. It allows you to query, visualize, alert on, and explore your metrics no matter where they are stored. In plain English, it provides you with tools to turn your time-series database (TSDB) data into beautiful graphs and visualizations.

* After creating a dashboard like you do in Getting started, there are many possible things you might do next. It all depends on your needs and your use case.

* For example, if you want to view weather data and statistics about your smart home, then you might create a playlist. If you are the administrator for a corporation and are managing Grafana for multiple teams, then you might need to set up provisioning and authentication.

Explore metrics and logs
=========================
* Explore your data through ad-hoc queries and dynamic drilldown. Split view and compare different time ranges, queries and data sources side by side.

Documentation
==============
https://www.fosslinux.com/10398/how-to-install-and-configure-prometheus-on-centos-7.htm

<img width="750" alt="Screenshot_541" src="https://user-images.githubusercontent.com/13994900/80279349-bc59ca80-86c2-11ea-9df8-7f4dd1084ef2.png">

Prerequistes
==============

* yum install ansible wget git -y 
* Python Version - Python 2.7.5 

Steps
======
1. git clone
2. ansible-playbook Prometheus+Grafana+Node_Exporter/Prometheus/grafana.yaml
3. http://Server-IP:3000/graph     #Take server Ip
4. <img width="750" alt="Screenshot_550" src="https://user-images.githubusercontent.com/13994900/80293549-0758f980-8726-11ea-9b10-90c7e40e2819.png">
5. Create Data Base
  <img width="750" alt="Screenshot_551" src="https://user-images.githubusercontent.com/13994900/80293555-1f307d80-8726-11ea-915b-b0c0aebd3326.png">
  6. Choose Prometheus 
  <img width="650" alt="Screenshot_552" src="https://user-images.githubusercontent.com/13994900/80293613-3ec7a600-8726-11ea-8094-9061b8e30aca.png">
7. Add Prometheus-Server-Ip:9090
<img width="600" alt="Screenshot_553" src="https://user-images.githubusercontent.com/13994900/80293619-4edf8580-8726-11ea-9307-a80f00ee4f26.png">
8.
