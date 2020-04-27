Prometheus
===========

Prometheus is a leading monitoring solution that has seen its community grow to large numbers. The support for multiple exporters is one of the strongest points of Prometheus, since it can help you get started with specific monitoring requirements quickly.

How does Prometheus  work ?
==========================
Prometheus is a leading open source monitoring and alerting tool. It had its origins at SoundCloud and has seen significant adoption since it was announced in 2015. The software was created because of the need to monitor multiple microservices that might be running in your system. Its architecture is modular and comes with several readily available modules called exporters, which help you capture metrics from the most popular software. Prometheus is written in the Go language, and it ships with easily distributed binaries that you can use to get it running as quickly as possible.

Documentation
==============


<img width="750" alt="Screenshot_541" src="https://user-images.githubusercontent.com/13994900/80279349-bc59ca80-86c2-11ea-9df8-7f4dd1084ef2.png">

Prerequistes
==============

* yum install ansible wget git 
* Python Version - Python 2.7.5 

Steps
======
1. git clone https://github.com/Taniusellu/ansible-playbooks-tatiana.git
2. ansible-playbook Prometheus+Grafana+Node_Exporter/Prometheus/Prometheus_install.yml

3. http://Server-IP:9090/graph     #Take server Ip

<img width="800" alt="Screenshot_543" src="https://user-images.githubusercontent.com/13994900/80281024-e2d13300-86cd-11ea-918e-e7f3d5147e2a.png">

4. Install Node_Exporter on different machine 
    * https://github.com/Taniusellu/ansible-playbooks-tatiana/tree/master/Prometheus%2BGrafana%2BNode_Exporter/Node_Exporter
    
5. vi /etc/prometheus/prometheus.yml
   * add the next task with your Ip- Node_Exporter
  <img width="450" alt="Screenshot_546" src="https://user-images.githubusercontent.com/13994900/80281593-e9fa4000-86d1-11ea-84d6-b39936e28ebe.png">
6.  systemctl restart prometheus

7. Collect CPU using the Node_Exporter 
<img width="650" alt="Screenshot_547" src="https://user-images.githubusercontent.com/13994900/80281646-43fb0580-86d2-11ea-95f7-87fc0650cd8f.png">


7. Take a Node_Exporter and Perform task on Grafana
<img width="350" alt="Screenshot_548" src="https://user-images.githubusercontent.com/13994900/80281703-a81dc980-86d2-11ea-9ff9-14e79a94d556.png">

8. Find more info about Grafana on this link #Grafana playbook
