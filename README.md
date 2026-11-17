# Vprofile_Project
##This My project:
<img width="1265" height="886" alt="image" src="https://github.com/user-attachments/assets/f1d4ecb6-5afb-455d-8706-81017cbe9ae1" />

##for Making Project like this: 
1- we go to make a security group so i do the following 
- go to EC2 > Security group in the Network & security > create security rule
<img width="1615" height="652" alt="image" src="https://github.com/user-attachments/assets/b8c38cef-3f39-4666-844c-5da4ee27a246" />
this for load balancer i make security group for it
<img width="1601" height="687" alt="image" src="https://github.com/user-attachments/assets/1c597895-a000-4e8b-8d9d-f4f300d561f3" />
this security group for Mysql (Port 3306) ,mmcache (Port 11211) & RabbitMQ (Port 5672) which i allowing to communicate with each other and gather traffic and also from tomcat instances
<img width="1596" height="592" alt="image" src="https://github.com/user-attachments/assets/346275eb-3da0-47b0-8612-78eed581d92e" />
this is the security group for tomcat instances that traffic go to from load balancer to it in the port 8080
