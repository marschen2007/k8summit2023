# k8summit2023
# NGINX 敏捷部署實戰：作為Ingress Controller（搭配EKS)

請填表單輸入您的email address,我們將發送email 給您開啟Lab

https://docs.google.com/forms/d/e/1FAIpQLSfw0qi-3ZW9y_xFH3FYtzOSmTJ8pA8s8tdbey1UjHKMgZy1PQ/formResponse

交付現代應用提高了提供不受基礎設施限制的敏捷應用服務的需求，同時確保應用運行得更快、安全且大規模部署。為應用程序選擇正確的架構可以讓組織更快地進行創新，並在任何基礎設施或雲架構上部署新服務。從代碼開發到客戶使用，部署在 AWS雲平台上的 NGINX 正在幫助企業交付應用基礎設施和服務，確保其應用快速、安全並大規模運行。

在本次研討會中，您將體驗如何以敏捷的方式部署應用，使用NGINX在AWS 雲平台，以完全自動化的方式使用所需的所有應用服務，例如API 管理和Web 應用防火牆"
K8s導入實戰 K8s架構設計   雲端原生架構

1. 使用 Terraform 部署 NGINX 基礎設施 -首先使用自動化並使用基礎架構即代碼概念來部署環境。
2. 使用 Kubernetes Nginx Ingress 提高可用性、安全性和應用性能
3. 使用 OpenID Connect 對用戶進行身份驗證，並將身份驗證過程從應用卸載到 Nginx
4. 零信任 -使用 NGINX 應用相互 TLS 身份驗證
5. 安全 -使用 Nginx App Protect Web 應用防火牆保護您的應用程序。"

## K8s 與NGINX 
使用 Terraform 部署 NGINX 基礎設施 -首先使用自動化並使用基礎架構即代碼概念來部署環境。
## NGINX基礎部署	
使用 Kubernetes Nginx Ingress 提高可用性、安全性和應用性能
## NGINX 安全功能部署	
- 使用 OpenID Connect 對用戶進行身份驗證，並將身份驗證過程從應用卸載到 Nginx
- 零信任 -使用 NGINX 應用相互 TLS 身份驗證
- 安全 -使用 Nginx App Protect Web 應用防火牆保護您的應用程序

本研討會將提供有關如何在 Amazon Elastic Kubernetes Service 環境中從頭開始部署應用程式的指南，同時使用 Nginx 解決方案保護和增強應用程式的可用性和可用性。

在本次研討會中，我們將使用「Arcadia Crypto」應用程式。 該應用程式由部署在 Kubernetes 環境中的 6 個不同的微服務建置。

在研討會結束時，「Arcadia Crypto」將得到全面部署和保護，如下圖所示。

研討會的文件可以在以下位置找到： 
http://udf.nginx-experience.com/

相關yaml檔案，請參考
https://github.com/sorinboia/nginx-experience-aws-ac2.0

步驟
1. 依流程啟動 UDF lab
2. web shell into the Jumpbox and start the lab while in the /home/ubuntu directory.
3. 執行以下指令
su ubuntu

cd /home/ubuntu

請忽略前兩章。 從第 3 章「Arcadia 部署」開始。

當環境啟動時，它將自動在 AWS 上部署基礎架構（第 2 章「Nginx 與 Terraform」）。
!!! 您需要等待 terraform 完成才能開始！
從部署開始起，這將需要 15 - 20 分鐘。 觀察日誌，當列印“ALL IS DONE”時，您就可以開始了。

tail -f /home/ubuntu/startup/startup.log
