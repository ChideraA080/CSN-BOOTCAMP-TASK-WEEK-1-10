
# AWS IDENTITY CENTER & PERMISSION SETS

This task involved configuring **AWS Identity Center** to manage user access within my AWS account. As part of the requirement, I created a new user and assigned the **SecurityAudit** job function policy using a permission set.

The goal was to understand how to use AWS Identity Center to apply fine-grained access control for users, following best practices around identity and permissions.


## WHAT I DID

- I enabled AWS Identity Center in the AWS Console.
- I created a new user with login credentials.
- I created and assigned a permission set using the predefined **SecurityAudit** policy.
- I verified that the user had limited security auditing access as expected.

## DELIVERABLES
- Screenshot of Identity Instance Center Created.
- Screenshot user created and assigned permission set.


## SCREENSHOTS
- Identity center instance created.
![Identity Center Instance](https://github.com/ChideraA080/CSN-Bootcamp-Week-2-Task-AWS-Identity-Center/blob/main/CSN%20BOOTCAMP%20WEEK%202/CSN%20BOOTCAMP%20WEEK%202.IDENTITY%20CENTER%20INSTANCE.png)
- Permission set created.
![Permission Set](https://github.com/ChideraA080/CSN-Bootcamp-Week-2-Task-AWS-Identity-Center/blob/main/CSN%20BOOTCAMP%20WEEK%202/CSN%20BOOTCAMP%20WEEK%202.%20PERMISSION%20SETS.png)

- User created and assigned permission set.
![User with assigned permission set](https://github.com/ChideraA080/CSN-Bootcamp-Week-2-Task-AWS-Identity-Center/blob/main/CSN%20BOOTCAMP%20WEEK%202/CSN%20BOOTCAMP%20WEEK%202%20(USER%20%26%20PERMISSION).png)

- Confirmation to test whether the user I created can create any resources using Ec2 instance for the test .And it failed to create an instance confirming that the assigned permission set is active as I gave Read Only Access to the user but not to create .

![Failed EC2 Confirmation](https://github.com/ChideraA080/CSN-Bootcamp-Week-2-Task-AWS-Identity-Center/blob/main/CSN%20BOOTCAMP%20WEEK%202/CSN%20BOOTCAMP%20WEEK%202.%20EC2%20INSTANCE%20FAILED%20DUE%20TO%20ASSIGNED%20PERMISSION%20SET.png)
## LESSONS LEARNED
- I learnt how to activate and configure AWS Identity Center.
- I understood the importance of managing user access securely in cloud environments.
- I gained practical experience with permission sets and job function policies in AWS.
- I saw how predefined policies like SecurityAudit help enforce the principle of least privilege.
