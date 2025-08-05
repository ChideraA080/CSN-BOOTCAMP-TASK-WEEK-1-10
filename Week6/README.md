DESCRIPTION OF WHAT I DID FOR WEEK 6.

# DEPLOYING METABASE WITH ECS AND RDS

In this task, I deployed **Metabase** using Amazon ECS Fargate and connected it to a **PostgreSQL database** hosted on Amazon RDS. The Metabase Docker image was pulled from Docker Hub, and necessary environment variables were configured to enable communication with the RDS instance. Both ECS and RDS resources were placed in the same VPC, with appropriate security group settings to allow traffic on port 5432.

## WHAT I DID

- I created a PostgreSQL database on Amazon RDS.
- I deployed Metabase as a task using **ECS with the Fargate launch type**.
- I pulled the official Metabase Docker image and set environment variables.
- I ensured both ECS and RDS were in the same VPC.
- I configured **RDS Security Group** to allow inbound traffic from ECS on port `5432`.
- I verified successful connection between Metabase and the RDS instance.

  ## DELIVERABLES
- Screenshot of RDS PostgreSQL Instance
- Screenshot of Task Defintion and Service running

- Screenshot of created Security Group allowing port 5432.

- Screenshot showing Task status as RUNNING.

- Screenshot of PostgreSQL being accessed externally

  ## SCREENSHOTS

# RDS POSTGRESQL INSTANCE DETAILS
![RDS PostgreSQL Instance](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week6/CSN%20BOOTCAMP%20WEEK%206%20TASK/CSN%20BOOTCAMP%20WEEK%206%20RDS%20INSTANCE.png)

# ECS TASK DEFINITION SUCCESSFULLY CREATED
![ECS Task definition](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week6/CSN%20BOOTCAMP%20WEEK%206%20TASK/CSN%20BOOTCAMP%20WEEK%206%20ECS%20TASK%20DEFINITION.png)

# RUNNING SERVICE SHOWING ACTIVE/SUCCESS
![Running Service](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week6/CSN%20BOOTCAMP%20WEEK%206%20TASK/CSN%20BOOTCAMP%20WEEK%206%20ECS%20SERVICE%20RUNNING.png)

# TASK DEFINITION WITH RUNNIG SERVICE
![Task definition with Service Running](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week6/CSN%20BOOTCAMP%20WEEK%206%20TASK/CSN%20BOOTCAMP%20WEEK%206%20TASK%20DEFINITION%20AND%20SERVICE%20RUNNING.png)

# SECURITY GROUP RULE TO ALLOW TRAFFIC FROM ECS TO RDS ON PORT 5432
![Security Group Rule for RDS](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week6/CSN%20BOOTCAMP%20WEEK%206%20TASK/CSN%20BOOTCAMP%20WEEK%206%20SG%20ON%20PORT%205432.png)

# SECURITY GROUP RULE TO ALLOW TRAFFICE TO METABASE ON PORT 3000)

![Security Group Rule for Metabase](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week6/CSN%20BOOTCAMP%20WEEK%206%20TASK/CSN%20BOOTCAMP%20WEEK%206%20SG%20ON%20PORT%203000.png)

# METABASE WELCOME PAGE
![Metabase Welcome page](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week6/CSN%20BOOTCAMP%20WEEK%206%20TASK/CSN%20BOOTCAMP%20WEEK%206%20METABSE%20WELCOME%20PAGE%201.png)

# METABASE PAGE SHOWING SUCCESSFUL CONNECTION TO DATABASE
![Metabase Page Successful Connection to Database](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week6/CSN%20BOOTCAMP%20WEEK%206%20TASK/CSN%20BOOTCAMP%20WEEK%206%20METABASE%20SUCCESSFUL%20CONNECTION%20TO%20DATABASE.png)


## LESSON LEARNED

- I learnt how to deploy and manage containerized applications using Amazon ECS Fargate.
- I gained experience in configuring Amazon RDS and enabling secure connectivity.
- I understood the importance of VPC networking and security group rules for inter-service communication.
- I practiced real-world use cases of connecting services (ECS) to managed databases (RDS).

