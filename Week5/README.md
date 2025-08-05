DESCRIPTION OF WHAT I DID FOR WEEK 5.

 DEPLOYING GRAFANA ON AMAZON ECS WITH FARGATE

Task Description
In this project, I deployed Grafana (a popular open-source dashboard and monitoring tool) on Amazon ECS with Fargate. The Grafana service runs on port 3000.  

The deployment involved:
- Using the official Docker image grafana/grafana.
- Creating a task definition exposing port 3000.
- Running the service in a public subnet.
- Configuring the security group to allow inbound traffic on port 3000.

Grafana Default Credentials
- Username: admin  
- Password: admin

Once deployed, I accessed Grafana via:  
http://<PUBLIC-IP>:3000

## DELIVERABLES
- ECS cluster and running service screenshots.
- Task definition showing grafana/grafana image.
- Security group rule for port 3000.
- Screenshot of Grafana login page.

  
## SCREENSHOTS

# ECS CLUSTER AND RUNNING SERVICE
![ECS Cluster & Running Service](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week5/CSN%20BOOTCAMP%20WEEK%205%20TASK/CSN%20BOOTCAMP%20WEEK%205%20ECS%20CLUSTER%20%26%20RUNNING%20SERVICE.png)

# GRAFANA SERVICE DEPLOYMENT STATUS
![Grafana Service Deployment status](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week5/CSN%20BOOTCAMP%20WEEK%205%20TASK/CSN%20BOOTCAMP%20WEEK%205%20%20GRAFANA%20SERVICE%20DEPLOYMENT%20STATUS.png)

# TASK DEFINITION SHOWING GRAFANA/GRAFANA IMAGE
![Task definition with grafana/grafana image](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week5/CSN%20BOOTCAMP%20WEEK%205%20TASK/CSN%20BOOTCAMP%20WEEK%205%20TASK%20DEFINITION%20WITH%20GRAFANA%20IMAGE.png)

# SECURITY GROUP RULE ALLOWING PORT 3000
![Security Group rule](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week5/CSN%20BOOTCAMP%20WEEK%205%20TASK/CSN%20BOOTCAMP%20WEEK%205%20SECURITY%20GROUP%20ALLOWING%20PORT%203000.png)

# GRAFANA WELCOME PAGE
![grafana Welcome Page](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week5/CSN%20BOOTCAMP%20WEEK%205%20TASK/CSN%20BOOTCAMP%20WEEK%205%20GRAFANA%20WELCOME%20PAGE%20%20WITH%20LOGIN%20DETAILS.png)

# GRAFANA LOGIN PAGE
![grafana Login Page](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week5/CSN%20BOOTCAMP%20WEEK%205%20TASK/CSN%20BOOTCAMP%20WEEK%205%20GRAFAN%20LOGIN%20PAGE%20IN%20BROWSER.png)


## LESSONS LEARNED
Lessons Learned
- I Understood how to create and manage an ECS Fargate cluster.
- I learned how to define and run tasks with custom Docker images.
- I practiced configuring security groups and public access.
- I gained hands-on experience with exposing and accessing services running in containers on AWS.

