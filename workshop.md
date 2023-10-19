This workshop will provide guidelines on how to deploy an application from scratch in Amazon Elastic Kubernetes Service environment while protecting and enhancing the application availability and usability with Nginx solutions.

For this workshop we are going to use the “Arcadia Crypto” application. The application is built with 6 different microservices that are deployed in the Kubernetes environment.

By the end of the workshop the “Arcadia Crypto” will be fully deployed and protected as described in the bellow diagram.

Documentation for the workshop can be found at:
http://udf.nginx-experience.com/

ssh into the Jumpbox and start the lab while in the /home/ubuntu/lab/ directory.

Ignore the first two chapters.
Start at chapter 3 "Arcadia deployment".

When the environment is started it will automatically deploy the infrastructure on AWS (chapter 2 "Nginx with Terraform").
!!! You will need to wait for terraform to finish before starting !!!
This will take 15 - 20 minutes from the moment the deployment is started.
Watch the logs and when "ALL IS DONE" is printed you can start.
tail -f /home/ubuntu/startup/startup.log

Nginx versions used at the moment:
KIC 1.11.1 with App Protect and Opentracing for Zipkin
Controller 3.16
Nginx+ R23 
