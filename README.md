Java WebApp DevOps Project 
==> Project Overview

This project demonstrates end-to-end DevOps workflow for a Java web application.

The application is containerized using Docker and deployed locally using Tomcat.

##### Tech Stack #####
.Java
.Maven
.Apache Tomcat
.Docker
.GitHub
.Jenkins (CI/CD – In Progress)


==> Build Steps (Local)
mvn clean package
WAR file will be generated inside the target/ directory.

==> Docker Build & Run
Build Docker Image
docker build -t java-webapp .
Run Container
docker run -d -p 8082:8080 --name javaapp java-webapp

Access Application
Open in browser:
http://localhost:8082
==> Automation Script
Local deployment automation using shell script:

./run.sh

This script performs:
.Maven Build
.Docker Image Build
.Stop Old Container
.Run New Container

CI/CD Pipeline (Work in Progress)

Jenkins pipeline is being configured to automate:
.Code Clone from GitHub
.Maven Build
.Docker Image Creation
.Container Deployment
<img width="1792" height="1120" alt="Screenshot 2026-03-24 at 12 38 56 PM" src="https://github.com/user-attachments/assets/280c4555-3ee7-4ced-9aab-8593ecc88859" />
<img width="1792" height="1120" alt="Screenshot 2026-03-24 at 12 39 37 PM" src="https://github.com/user-attachments/assets/56863c4c-8cce-48a9-9986-dc3808568fb1" />
<img width="1792" height="1120" alt="Screenshot 2026-03-24 at 12 41 02 PM" src="https://github.com/user-attachments/assets/b1349818-c03c-44d9-8b67-7de3efb9ac0d" />
<img width="1779" height="980" alt="Screenshot 2026-03-24 at 12 40 44 PM" src="https://github.com/user-attachments/assets/42c23cb2-6901-44b4-93b7-7aa3a8af024d" />
<img width="1782" height="1047" alt="Screenshot 2026-03-24 at 12 53 31 PM" src="https://github.com/user-attachments/assets/16b6c437-36d5-4171-9d35-fc10cda689e0" />
<img width="1792" height="1120" alt="Screenshot 2026-03-24 at 1 00 19 PM" src="https://github.com/user-attachments/assets/281e7eac-a054-4df3-8590-300e917a3531" />
<img width="1786" height="1056" alt="Screenshot 2026-03-24 at 1 00 49 PM" src="https://github.com/user-attachments/assets/1099ea59-550b-44ab-93a6-1e876e327eac" />
<img width="1792" height="1120" alt="Screenshot 2026-03-24 at 1 00 54 PM" src="https://github.com/user-attachments/assets/4b0337da-6fdb-4ab3-8776-24779801e190" />
<img width="1792" height="1120" alt="Screenshot 2026-03-24 at 1 00 54 PM" src="https://github.com/user-attachments/assets/6ed91003-eef8-4fe5-ae33-13e3128808a0" />







