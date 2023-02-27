# GCP-petclinic-3-Tier-with-Console
* Reservation service using GCP(petclinic)

* Period ➛ 2022.08.29 ~ 2022.09.16
* Personnel ➛5

----
## 0. Project requirements(Detail)
- WEB Server : Apache v2.4.37
- WAS Server : Tomcat v9.0.64(내장)
- WEB, WAS 연동 : mod_proxy
- DB : MySQL(v8.0)
- Cloud DNS : www.petclinic.shop
- Cloud CDN : GCS(Google Cloud Storage)
- Cloud Monitoring
- Autoscale

----
## 1. Architecture
### 1.1 Large Architecture
![image](https://user-images.githubusercontent.com/110655818/217455948-ba5885d6-572b-40ae-aa81-c20de9a22297.png)

### 1.2 Architecture for End Users
![image](https://user-images.githubusercontent.com/110655818/217456235-58809f04-17f8-422d-b11c-f1f1cc1c9bbe.png)

### 1.3 Architecture for Admin
![image](https://user-images.githubusercontent.com/110655818/217456380-46563681-f07e-4e43-bbfe-3e0a3e624ab8.png)

---
## 2. Architecture 세부사항
### 2.1 VPC Network (VPC&Subnet)
![image](https://user-images.githubusercontent.com/110655818/217457101-ef70f16d-36e3-429b-8033-18a3c8635afc.png)

### 2.2 VPC Network (Firewall)
![image](https://user-images.githubusercontent.com/110655818/217457181-5723929e-ef67-447d-bc67-34d8f71176a1.png)

### 2.3 Cloud SQL
![image](https://user-images.githubusercontent.com/110655818/217457303-630a17aa-3f7c-4b58-9ab5-b28a43a34060.png)

### 2.4 Compute Engine (VM Instance)
![image](https://user-images.githubusercontent.com/110655818/217457417-03cff25d-4cf8-4177-868d-74b49840db3e.png)

### 2.5 Compute Engine (Snapshot, Image, Template)
![image](https://user-images.githubusercontent.com/110655818/217457654-df4819dc-2469-49a2-9144-d7e846b6d31c.png)

### 2.6 Compute Engine (Instance Groups)
![image](https://user-images.githubusercontent.com/110655818/217457753-fbeec6a1-8180-4744-8df0-4ed261b0c57e.png)

### 2.7 Load Balancer (internal load balancer)
![image](https://user-images.githubusercontent.com/110655818/217458037-0da2d8c4-1ccc-4c63-9645-655e86418978.png)

### 2.8 Load Balancer (external load balancer)
![image](https://user-images.githubusercontent.com/110655818/217458278-f5f1a74a-5fe9-4d5f-a14e-3099f60436da.png)

### 2.9 DNS
![image](https://user-images.githubusercontent.com/110655818/217458425-8c1309db-b516-444f-ac66-ac706405d0fc.png)

### 2.10 GCS (Google Cloud Storage)
![image](https://user-images.githubusercontent.com/110655818/217458537-04027f95-113f-4017-abeb-37f5bb64bf78.png)

----
## 3. Tests and Results
### 3.1 Web Page access and DB Check
![image](https://user-images.githubusercontent.com/110655818/217458946-bb745c07-e253-4e92-9494-08ce667f62c9.png)

### 3.2 Jmeter, Monitoring
(Video) https://docs.google.com/file/d/1cVF4VDimuIINZPNcgVsBknFuUFzsdOrI/preview

----
## 4. Reference
https://judy-nick.notion.site/GCP-petclinic-3-Tier-with-Console-fc308b837ea54e9eae15eead79a4e35d
