DESCRIPION OF WHAT I DID FOR WEEK 4.

# AWS VPC PEERING AND SUBNET CONFIGURATION

This task involved creating a multi-VPC architecture in AWS by provisioning two separate VPCs (`VPC-A` and `VPC-B`) with their own CIDR blocks. Each VPC was configured with a public and private subnet. I then established a VPC peering connection between them and updated route tables to allow traffic flow between both VPCs.

## WHAT I DID
- I created `VPC-A` with CIDR block `10.10.0.0/16` and `VPC-B` with `10.20.0.0/16`.
- I configured one public and one private subnet in each VPC.
- I established a **VPC peering connection** between `VPC-A` and `VPC-B`.
- I updated route tables in both VPCs to enable communication across the peering link.
- I verified peering connection was in **Active** state.


## SCREENSHOTS

# VPC-A CIDR BLOCK
![VPC-A CIDR BLOCK](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week4/CSN%20BOOTCAMP%20WEEK%204%20TASK/CSN%20BOOTCAMP%20WEEK%204%20VPC%20-A%20WIT%20CIDR%20BLOCK.png)

# VPC-B CIDR BLOCK
![VPC-B CIDR BLOCK](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week4/CSN%20BOOTCAMP%20WEEK%204%20TASK/CSN%20BOOTCAMP%20WEEK%204%20VPC%20-B%20WITH%20CIDR%20.png)

# VPC-A PUBLIC SUBNET
![VPC-A PUBLIC SUBNET](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week4/CSN%20BOOTCAMP%20WEEK%204%20TASK/CSN%20BOOTCAMP%20WEEK%204%20VPC%20-A%20PUBLIC%20SUBNET%20AND%20CIDR.png)

# VPC-A PRIVATE SUBNET
![VPC-A PRIVATE SUBNET](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week4/CSN%20BOOTCAMP%20WEEK%204%20TASK/CSN%20BOOTCAMP%20WEEK%204%20VPC%20-A%20PRIVATE%20SUBNET%20AND%20CIDR.png)

# VPC-B PUBLIC SUBNET
![VPC-B PUBLIC SUBNET](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week4/CSN%20BOOTCAMP%20WEEK%204%20TASK/CSN%20BOOTCAMP%20WEEK%204%20VPC%20-B%20PUBLIC%20SUBNET%20WITH%20CIDR.png)

# VPC-B PRIVATE SUBNET
![VPC-B PRIVATE SUBNET](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week4/CSN%20BOOTCAMP%20WEEK%204%20TASK/CSN%20BOOTCAMP%20WEEK%204%20VPC%20-B%20PRIVATE%20SUBNET%20AND%20CIDR.png)

# VPC-A ROUTE TABLE
![VPC-A ROUTE TABLE](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week4/CSN%20BOOTCAMP%20WEEK%204%20TASK/CSN%20BOOTCAMP%20WEEK%204%20VPC%20-A%20ROUTE%20TABLE.png)

# VPC-A ROUTE TABLE
![VPC-A ROUTE TABLE](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week4/CSN%20BOOTCAMP%20WEEK%204%20TASK/CSN%20BOOTCAMP%20WEEK%204%20VPC-A%20ROUTE%20TABLES.png)

# VPC-B ROUTE TABLE
![VPC-B ROUTE TABLE](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week4/CSN%20BOOTCAMP%20WEEK%204%20TASK/CSN%20BOOTCAMP%20WEEK%204%20VPC-B%20ROUTE%20TABLES.png)

# VPC-B ROUTE TABLE
![VPC-B ROUTE TABLE](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week4/CSN%20BOOTCAMP%20WEEK%204%20TASK/CSN%20BOOTCAMP%20WEEK%204%20VPC%20-B%20ROUTE%20TABLE.png)

# VPC PEERING ACTIVE STATUS
![VPC PEERING ACTIVE STATUS](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week4/CSN%20BOOTCAMP%20WEEK%204%20TASK/CSN%20BOOTCAMP%20WEEK%204%20VPC%20PEERING%20ACTIVE%20STATUS(VPC%20-A%20TO%20VPC%20-B).png)

# VPC-A TO VPC-B PEERING CONNECTION
![VPC-A TO VPC-B PEERING CONNECTION](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week4/CSN%20BOOTCAMP%20WEEK%204%20TASK/CSN%20BOOTCAMP%20WEEK%204%20VPC-A%20TO%20VPC-B%20PEERING%20CONNECTION%20IN%20ACTIVE%20STATUS.png)

## LESSONS LEARNED
- I gained hands-on experience with **custom VPC creation and subnetting** in AWS.
- I learnt how to set up and validate **VPC peering connections** for inter-VPC communication.
- I understood the role of **route tables** in controlling traffic between VPCs.
- I reinforced the concept of **network isolation and secure interconnection** in cloud environments.
