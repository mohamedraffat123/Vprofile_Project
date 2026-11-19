# Vprofile_Project
## This My project:
<img width="1265" height="886" alt="image" src="https://github.com/user-attachments/assets/f1d4ecb6-5afb-455d-8706-81017cbe9ae1" />

## for Making Project like this: 
1- we go to make a security group so i do the following 
  - go to EC2 > Security group in the Network & security > create security rule
  <img width="1615" height="652" alt="image" src="https://github.com/user-attachments/assets/b8c38cef-3f39-4666-844c-5da4ee27a246" />
  this for load balancer i make security group for it
  <img width="1601" height="687" alt="image" src="https://github.com/user-attachments/assets/1c597895-a000-4e8b-8d9d-f4f300d561f3" />
  this security group for Mysql (Port 3306) ,mmcache (Port 11211) & RabbitMQ (Port 5672) which i allowing to communicate with each other and gather traffic and also from tomcat instances
  <img width="1596" height="592" alt="image" src="https://github.com/user-attachments/assets/346275eb-3da0-47b0-8612-78eed581d92e" />
  this is the security group for tomcat instances that traffic go to from load balancer to it in the port 8080
2- we go to instance to make database here
  - go to EC2 > instances > launch an instances
    <img width="1193" height="435" alt="image" src="https://github.com/user-attachments/assets/dae6f6c7-25e5-4f4f-9182-ffd4b1b86c75" />
    <img width="1221" height="468" alt="image" src="https://github.com/user-attachments/assets/5b28b15f-2523-4e1d-b182-789ff02a7354" />
    Here i use AWS as we deal with database but later we use ubuntu for tomcat but for now we use Amazon Linux 2023 (kernel-6.18)AMI
    <img width="1145" height="272" alt="image" src="https://github.com/user-attachments/assets/02ea75e5-511e-4fb8-bbe5-a6f88f45ba5d" />
    Here we use the KeyPair that we download it and made it is Vprofile-prod-key
    <img width="1045" height="617" alt="image" src="https://github.com/user-attachments/assets/2df18d9a-c7b0-4526-ab9f-2687ef21242c" />
    Here is the network Security and select "Select existing security" group we put in the common Security group the Group of backend as it contain the MySql
    <img width="882" height="581" alt="image" src="https://github.com/user-attachments/assets/964f952c-2920-451c-a081-5cbddc1c7f9f" />
    Then go to advanced option and at the end put the code of bash for making database as it exist in the code
    <img width="1908" height="335" alt="image" src="https://github.com/user-attachments/assets/e13aabb6-ffe2-437e-bff5-7ff1a75caa69" />
    Then Launch it and we will do the same for mmcache and RabbitMQ as above but the difference here we put the difference code for each one of them
    but for tomcat there is a little change we use ubuntu not AWS AMI
    <img width="1225" height="572" alt="image" src="https://github.com/user-attachments/assets/a92dfdd1-d4b0-49d0-b678-3b63187ac7b1" />
    make sure that you use Ubuntu Server 24.04 LTS (HVM) 



