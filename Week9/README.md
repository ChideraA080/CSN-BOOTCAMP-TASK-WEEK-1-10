# DESCRIPTION OF WHAT I DID IN TASK 9

# SIMULATED DOMAIN, SSL & CDN SETUP (SIMULATED)

## Task Expectations
The task was to:
- Host a static website on **Amazon S3**.
- Connect it to a **custom domain** (via Route 53 or another DNS provider).
- Request an **SSL certificate** in AWS Certificate Manager (ACM).
- Use **CloudFront** to distribute content securely over HTTPS.
- Redirect all HTTP traffic to HTTPS.

  ## WHAT I DID (SIMULATION)
Since I’m on AWS Free Tier and Freenom (free domain provider) was down, I **simulated** the process instead of deploying live to avoid costs:

- I created an S3 bucket `csn-week9-task`, enabled **Static Website Hosting**, uploaded a sample `index.html`, and Set Bucket Policy to allow **public read access**.
- I assumed a custom domain name `demoapp123.tk` for simulation.
- I requested a **public SSL certificate** for `demoapp123.tk` in ACM (DNS validation) but left it **Pending**.
- I documented how I would connect the domain via DNS records if Freenom was available as **I did not** create a **Route 53 hosted zone** (to avoid charges).
- Simulated CloudFront setup with:
  - Origin = S3 bucket
   Went to CloudFront > Create Distribution
  - Selected: Single website or app
  - Set Origin to: csn-week9-task.s3.amazonaws.com (REST endpoint)
  - I did NOT use S3 website endpoint (to ensure HTTPS works)
- **I did not** create CloudFront distribution or Route 53 records to avoid charges.

  ## WHAT I WOULD HAVE DONE IF FREENOM WAS AVAILABLE

```Custom Domain & HTTPS (Simulated Setup)```

Since Freenom (free domain provider) was temporarily down, I couldn’t register an actual custom domain. Instead, I simulated using a free domain called demoapp123.tk for the task.

- Registered a free domain (e.g., demoapp123.tk) via Freenom.com.

- Configured the domain’s DNS settings to point to my CloudFront distribution using a CNAME record.

- Used AWS Certificate Manager (ACM) to request a public SSL certificate for demoapp123.tk using DNS validation.

- Validated the certificate by adding the CNAME record provided by AWS to Freenom's DNS panel.

- Attached the validated SSL certificate to the CloudFront distribution.

  ## DELIVERABLES

- `index.html` | Sample webpage hosted on S3 .
-  Screenshot – S3 | Static hosting enabled + public policy .
-  Screenshot – ACM | Certificate request (Pending Validation) .
-  Screenshot – CloudFront | Simulated HTTPS + custom domain settings .
-  README.md | This documentation .

  ## SCREENSHOTS

  # S3 STATIC WEBSITE HOSTING ENABLE
![Static Website Hosting Enabled](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week9/CSN%20BOOTCAMP%20WEEK%209%20TASK/CSN%20BOOTCAMP%20WEEK%209%20STATIC%20HOSTING%20ENABLED.png)

# BUCKET POLICY USED
![Bucket Policy](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week9/CSN%20BOOTCAMP%20WEEK%209%20TASK/CSN%20BOOTCAMP%20WEEK%209%20BUCKET%20POLICY.png)

# HTML DISPLAY UPLOADED FILE ON WEBPAGE
![Html file uploaded](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week9/CSN%20BOOTCAMP%20WEEK%209%20TASK/CSN%20BOOTCAMP%20WEEK%209%20NOT%20SECURE%20HTML%20DISPLAY%20PAGE.png)

# FREENOM SITE SIMULATION
![Freenom Domain Site Simulated](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week9/CSN%20BOOTCAMP%20WEEK%209%20TASK/CSN%20BOOTCAMP%20WEEK%209%20FREENOM%20DEMO%20APP.png)

# HOSTED ZONE SIMULATION
![Hosted Zone Simulated](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week9/CSN%20BOOTCAMP%20WEEK%209%20TASK/CSN%20BOOTCAMP%20WEEK%209%20HOSTED%20ZONE%20SIMULATION.png)

# ACM CERTIFICATE PENDING VALIDATION
![ACM Certificate Pending Request](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week9/CSN%20BOOTCAMP%20WEEK%209%20TASK/CSN%20BOOTCAMP%20WEEK%209%20CERTIFICATE%20MANAGER%20REQUEST%20.png)

# CLOUD FRONT DISTRIBUTION SIMULATION
![Cloudfront Distribution Simulated](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week9/CSN%20BOOTCAMP%20WEEK%209%20TASK/CSN%20BOOTCAMP%20WEEK%209%20CLOUDFRONT.png)


## NOTES

- I did **not create a Route 53 Hosted Zone** to avoid AWS charges.
- I did **not complete domain registration on Freenom** (service was unavailable).
- I did **not create the CloudFront distribution**, only simulated the setup.

    
## LESSONS LEARNED
- How to host a static website using Amazon S3.
- How SSL certificates are requested via AWS Certificate Manager.
- How CloudFront can distribute S3 content securely over HTTPS.
- Importance of REST endpoint vs. Website endpoint for SSL.
- How to simulate Route 53 setup using a custom domain name without incurring cost.
- Safe practices for Free Tier AWS usage.


  
