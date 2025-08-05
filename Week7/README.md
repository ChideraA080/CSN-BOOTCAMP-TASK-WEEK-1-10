DESCRIPTION OF WHAT I DID FOR WEEK 7.

# MONITORING & OBSERVABILITY WITH CLOUDWATCH
In this task, I deployed a simple containerized application (Nginx) on Amazon ECS using Fargate, selecting appropriate CPU and memory configurations. The service was launched in a public subnet, and I created a CloudWatch dashboard to monitor key metrics in real time.

I used CloudWatch widgets to track CPUUtilization and MemoryUtilization. To simulate traffic and analyze metric changes, I refreshed or stressed the application from a browser.

## WHAT I DID

- I created a simple Docker container using the **Nginx** image.
- I ceployed the container to **Amazon ECS** using the **Fargate launch type**.
- I configured CPU and memory values in the ECS Task Definition.
- I deployed the service in a **public subnet**.
- I created a **CloudWatch Dashboard** and added widgets for CPU and memory metrics.
-  I simulated load and observed metric fluctuations in the dashboard.

  ## DELIVERABLES

- Screenshot of ECS cluster and running service.
- Screenshot of ECS Task Definition showing CPU and memory configurations.
-  Screenshot of CloudWatch Dashboard showing:

    - `CPUUtilization` widget
  
   - `MemoryUtilization` widget
-  *(Optional)* Screenshot showing metric changes under simulated load.

  ## SCREENSHOTS
  
  # NGINX CLUSTER CREATED
![Nginx Cluster Running](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week7/CSN%20BOOTCAMP%20WEEK%207%20TASK/CSN%20BOOTCAMP%20WEEK%207%20%20NGINX%20CLUSTER%20RUNNING.png)

# ECS CLUSTER & RUNNING SERVICE
![ECS Cluster & Running Service](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week7/CSN%20BOOTCAMP%20WEEK%207%20TASK/CSN%20BOOTCAMP%20WEEK%207%20ECS%20CLUSTER%20AND%20RUNNING%20SERVICE.png)

# TASK DEFINITION WITH CPU & MEMORY SETTINGS
![Task Definition with CPU & Memory](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week7/CSN%20BOOTCAMP%20WEEK%207%20TASK/CSN%20BOOTCAMP%20WEEK%207%20TASK%20DEFINITION%20WITH%20CPU.png)

# NGINX WEBPAGE
![Nginx Webpage](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week7/CSN%20BOOTCAMP%20WEEK%207%20TASK/CSN%20BOOTCAMP%20WEEK%207%20NGINX%20WEBPAGE.png)

# CLOUDWATCH DASH BOARD SHOWING CPU & MEMORY WIDGETS
![Cloudwatch Dashboard with CPU & Memory Widgets](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week7/CSN%20BOOTCAMP%20WEEK%207%20TASK/CSN%20BOOTCAMP%20WEEK%207%20CLOUDWATCH%20DASHBOARD%20%20%26CPU.png)

# CHANGES UNDER SIMULATED LOAD
![Changes Under Simulated load](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week7/CSN%20BOOTCAMP%20WEEK%207%20TASK/CSN%20BOOTCAMP%20WEEK%207%20DASHBOARD%20UNDER%20SIMULATED%20LOAD.png)


## LESSONS LEARNED

- I gained hands-on experience monitoring ECS services using **AWS CloudWatch**.
- I learned how to configure and visualize **CPU and memory usage** for Fargate tasks.
- I understood how to create custom **CloudWatch Dashboards** with metric widgets.
- I observed how simulated load impacts resource usage, which is crucial for planning **auto-scaling** and resource provisioning.
