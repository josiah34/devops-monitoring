# devops-monitoring

In this project I will be setting up a web application on an ec2 image and monitoring it using Grafana, Prometheus and Alert Manager as a part of the DevOps Monitoring Deep Dive course on A Cloud Guru



1. I created a terraform script to quickly deploy my ec2 instance along with installing and setting up docker. 

![docker-1](https://github.com/josiah34/devops-monitoring/assets/25124463/31819a95-bb65-4618-be01-94b33ce9244b)

2. I then clone the example application ``https://github.com/linuxacademy/content-devops-monitoring-app``

![cloning-app-2](https://github.com/josiah34/devops-monitoring/assets/25124463/ebc03836-1144-45ad-bf00-ddf48cdf457e)

3. Next I will build the dockerfile ``docker build --tag web-app .`` to create the image of the web application. 
4. From that image I will then run a container ``docker run --name web-app -p 80:8080 -d web-app``\
5. To see the running app go to ``http://YOUR_PUBLIC_IP:80``
![running-app-3](https://github.com/josiah34/devops-monitoring/assets/25124463/b4e413f2-42e2-4f84-be48-849a237fcd24)

