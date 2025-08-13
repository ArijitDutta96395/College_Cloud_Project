# 🌩️ Cloud Computing Project – AWS AMI Replication & Application Redundancy  

## 📌 Overview  
This project demonstrates **creating a custom Amazon Machine Image (AMI)** from an existing **AWS EC2 instance**, copying it to another AWS region, and launching it to **test application redundancy**.  
It showcases how cloud computing can be leveraged to build **scalable, fault-tolerant, and region-independent applications**.  

---

## 👥 Team Members  
**Team Leader:** Arijit Dutta (22/ECE/54)  
**Members:**  
- Abhijit Nandi (22/ECE/018)  
- Girish Chandra Ghosh (22/ECE/080)  
- Jinat Kaderi (22/ECE/090)  
- Nibha Kumari (22/ECE/113)  
- Prasenjit Sarkar (22/ECE/127)  
- Soham Chowdhury (22/ECE/172)  
- Arghya Mandal (22/ECE/052)  
- Ayan Rakesh (22/ECE/062)  
- Dipan Das (22/ECE/074)  
- Esa Roy (22/ECE/078)  

---

## 🛠️ Technologies Used  
- **Amazon Web Services (AWS)** – EC2, AMI, S3, CloudWatch, Lambda  
- **React.js** – For front-end application hosting  
- **Node.js** – Backend runtime environment  
- **NGINX** – Web server for application hosting  
- **PM2** – Process manager for Node.js applications  

---

## 📂 Project Workflow  

### 1️⃣ Create a Custom AMI from a Running EC2 Instance  
1. Log in to AWS Management Console.  
2. Select EC2 instance → Actions → Image and Templates → Create Image.  
3. Provide AMI name & description.  
4. Monitor creation progress under **AMI section**.  

### 2️⃣ Copy the Custom AMI to Another AWS Region  
1. Navigate to **EC2 → AMIs**.  
2. Select AMI → Actions → Copy AMI.  
3. Choose **Destination Region**.  
4. Wait for the copy process to complete.  

### 3️⃣ Launch an Instance from the Copied AMI  
1. Switch to the **destination region**.  
2. Go to **EC2 → AMIs** and select the copied AMI.  
3. Launch the instance with required configurations.  

### 4️⃣ Test Application Redundancy  
- Deploy React app on the new instance.  
- Verify that the application is functional in both regions.  
- Conduct performance & availability tests.  

---

## 🌍 Deployment Details – Hosting React App on AWS EC2  
1. Install **Node.js** on Ubuntu server.  
2. Install **NGINX** and configure reverse proxy.  
3. Create React application and upload to server (via file manager/SCP).  
4. Use **PM2** to keep the app running persistently.  
5. Set correct **security group rules** for HTTP/HTTPS access.  

---

## ✅ Key Outcomes  
- **High Availability:** Application is live in multiple AWS regions.  
- **Fault Tolerance:** Failover possible in case of region outage.  
- **Scalability:** AMIs can be deployed in multiple regions as needed.  

---

## ⚠️ Challenges & Considerations  
- **Security & Privacy** – Ensuring compliance with cloud security best practices.  
- **Vendor Lock-in** – Avoiding over-dependence on AWS-specific tools.  
- **Reliability** – Maintaining uptime across multiple regions.  

---

## 📖 Key Takeaways  
- **Resilience**: AMI replication enables disaster recovery.  
- **Scalability**: Resources can be provisioned quickly in any AWS region.  
- **Best Practices**: Encourages redundancy, monitoring, and security.  

---

## 📜 License  
This project is for **educational purposes** and is not intended for production use without proper security hardening.  

---

## 🙏 Acknowledgement  
We sincerely thank our mentors **Dr. Chanchal Kumar De, Mr. Bidhan Acharya, Mr. Akinchan Das, and Mrs. Pallabi Pahari** for their constant support, guidance, and encouragement throughout this project.  
