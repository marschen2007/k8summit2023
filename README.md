# k8summit2023
# NGINX 敏捷部署實戰：作為Ingress Controller（搭配EKS)

交付現代應用提高了提供不受基礎設施限制的敏捷應用服務的需求，同時確保應用運行得更快、安全且大規模部署。為應用程序選擇正確的架構可以讓組織更快地進行創新，並在任何基礎設施或雲架構上部署新服務。從代碼開發到客戶使用，部署在 AWS雲平台上的 NGINX 正在幫助企業交付應用基礎設施和服務，確保其應用快速、安全並大規模運行。

工作坊簡介
在本次研討會中，您將體驗如何以敏捷的方式部署應用，使用NGINX在AWS 雲平台，以完全自動化的方式使用所需的所有應用服務，例如API 管理和Web 應用防火牆"
K8s導入實戰 K8s架構設計   雲端原生架構

1. 使用 Terraform 部署 NGINX 基礎設施 -首先使用自動化並使用基礎架構即代碼概念來部署環境。
2. 使用 Kubernetes Nginx Ingress 提高可用性、安全性和應用性能
3. 使用 OpenID Connect 對用戶進行身份驗證，並將身份驗證過程從應用卸載到 Nginx
4. 零信任 -使用 NGINX 應用相互 TLS 身份驗證
5. 安全 -使用 Nginx App Protect Web 應用防火牆保護您的應用程序。"


This workshop will provide guidelines on how to deploy an application from scratch in Amazon Elastic Kubernetes Service environment while protecting and enhancing the application availability and usability with Nginx solutions.

For this workshop we are going to use the “Arcadia Crypto” application. The application is built with 6 different microservices that are deployed in the Kubernetes environment.

By the end of the workshop the “Arcadia Crypto” will be fully deployed and protected as described in the bellow diagram.

Documentation for the workshop can be found at: http://udf.nginx-experience.com/

ssh into the Jumpbox and start the lab while in the /home/ubuntu/lab/ directory.

Ignore the first two chapters. Start at chapter 3 "Arcadia deployment".

When the environment is started it will automatically deploy the infrastructure on AWS (chapter 2 "Nginx with Terraform"). !!! You will need to wait for terraform to finish before starting !!! This will take 15 - 20 minutes from the moment the deployment is started. Watch the logs and when "ALL IS DONE" is printed you can start. tail -f /home/ubuntu/startup/startup.log

Nginx versions used at the moment: KIC 1.11.1 with App Protect and Opentracing for Zipkin Controller 3.16 Nginx+ R23
