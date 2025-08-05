DESCRIPTION OF WHAT I DID fOR WEEK 3.
# PROVISIONING AND SECURING A WINDOWS EC2 INSTANCE

This task involved launching a new Windows Server EC2 instance on AWS using the Windows Server 2019 Base AMI. I deployed the instance into a public subnet and configured a Security Group that allows RDP (port 3389)  access only from my public IP address.

I also assigned the instance a Name tag: `CSN-Bootcamp-Week3


## WHAT I DID
- I Launched a Windows Server 2019 EC2 instance.
- I deployed it into a public subnet within my VPC.
- I assigned the Name tag: `CSN-Bootcamp-Week3`.
- I created a Security Group that allows RDP access on port 3389 from my personal IP only.
- I connected successfully via Remote Desktop (RDP) and verified the connection.

## DELIVERABLES
- Screenshot of EC2 running instance
- screenshot of Security Group allowing RDP Port 3389.
- Screenshot of successfull emote Desktop (RDP) CONNECTION TO INSTANCE
  
## SCREENSHOTS

# Running Instance
![Running Instance](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week3/CSN%20BOOTCAMP%20WEEK%203/CSN%20BOOTCAMP%20WEEK%203.%20EC2%20RUNNING.png)
# Security Group
![Security Group](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week3/CSN%20BOOTCAMP%20WEEK%203/CSN%20BOOTCAMP%20WEEK%203.%20RDP%20SECURITY%20GROUP%20INBOUND%20RULES.png)
# Remote Desktop Connection
![Remote Desktop Connection](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week3/CSN%20BOOTCAMP%20WEEK%203/CSN%20BOOTCAMP%20WEEK%203.%20RDP%20REMOTE%20DESKTOP%20CONNECTION.jpg)

## LESSONS LEARNED
- I Learnt how to securely provision Windows EC2 instances in a public subnet.
- I Gained experience with Security Group configurations and restricting RDP access.
- I understood how to use Name tags and test remote desktop access using public IP restrictions.

