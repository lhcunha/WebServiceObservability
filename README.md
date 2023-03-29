# WebServiceObservability
On this project I explore observability by monitoring a webservice/API using the following stack: Prometheus, Grafana and AlertManager.

GOAL:

The objective of this project was to explore and demonstrate the monitoring capabilities of a stack composed by Prometheus, Grafana and AlertManager

PREREQUISITES:

- Java 1.8 or higher installed
- Maven installed
- Docker installed
- Docker Compose installed

The major steps followed on this project were:

- Created a basic webservice using Java Springboot
- Instrumented the webservice
- Outsourced the webservice's metrics using Spring's actuator
- Exposed those metrics to Prometheus using the Micrometer
- Created a shell script microservice to mimic a client who consumes the webservice
- Configured Grafana to use Prometheus as it's datasource.
- Created dashboards on Grafana to view those metrics on a fancy way
- Configured AlertManager to send alarms based on thresholds to a Slack channel


Here are some screenshots of the final result:

Grafana Dashboards:
![image](https://user-images.githubusercontent.com/19196422/228393376-25627b52-1ae1-4d40-87b6-549d48e98415.png)
![image](https://user-images.githubusercontent.com/19196422/228394138-1453d8d4-759a-4b3f-b3a7-256eee7c8f0e.png)

Application metrics:
![image](https://user-images.githubusercontent.com/19196422/228394998-d61d968e-79d8-4fa8-9db4-cf1eaa1557b6.png)

Prometheus Alerts:
![image](https://user-images.githubusercontent.com/19196422/228395271-ca1a7da8-76ad-4ad4-89c2-85bc51a75a1b.png)

Alerts sent to Slack channel via webhook:
![image](https://user-images.githubusercontent.com/19196422/228395567-30312f8c-1417-42bf-887b-39654f4f2deb.png)

