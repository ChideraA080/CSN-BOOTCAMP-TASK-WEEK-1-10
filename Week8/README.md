DESCRIPTION OF WHAT I DID FOR WEEK 8.

# STATIC WEBSITE HOSTING WITH AMAZON S3 & CLOUDFRONT
This task involved deploying a personal static website (resume/portfolio/About Me page) using Amazon S3 for storage and CloudFront for secure delivery. The goal was to host a simple HTML site publicly and deliver it securely via CloudFront.

## WHAT I DID
- I created an S3 bucket, uploaded index.html (About me) and enabled static website hosting  
- I set a bucket policy to allow public read access  
- I created a CloudFront distribution pointing to the S3 bucket as origin  
- I accessed the site using the CloudFront URL.

  
## DELIVERABLES
- Screenshot of S3 bucket showing static website hosting enabled. 
- Screenshot of bucket policy allowing public access. 
- Screenshot of CloudFront distribution settings and status.
- Screenshot of live website accessed via CloudFront domain.

  
## SCREENSHOTS

# BUCKET CONFIGURATION WITH STATIC WEBSITE ENABLED
![Bucket Configuration Showing Static website enabled](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week8/CSN%20BOOTCAMP%20WEEK%208%20TASK/CSN%20BOOTCAMP%20WEEK%208%20BUCKET%20CONFIG%20STATIC%20WEB%20HOSTING%20ENABLED.png)

# BUCKET ERROR PAGE WHEN URL WAS ACCESSED ON WEBPAGE BEFORE BUCKET POLICY WAS APPLIED
![Bucket Error Page before Bucket Policy](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week8/CSN%20BOOTCAMP%20WEEK%208%20TASK/CSN%20BOOTCAMP%20WEEK%208%20ERROR%20PAGE%20BEFORE%20BUCKET%20POLICY.png)

# BUCKET POLICY USED TO ALLOW PUBLIC ACCESS
![Bucket Policy](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week8/CSN%20BOOTCAMP%20WEEK%208%20TASK/CSN%20BOOTCAMP%20WEEK%208%20BUCKET%20POLICY.png)

# BUCKET SHOWING NOT SECURE WHEN ACCESSED WITH THE URL ENDPOINT AFTER BUCKET POICY WAS APPLIED
![Bucket Showing Not Secure When accessed Bucket Endpoint URL](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week8/CSN%20BOOTCAMP%20WEEK%208%20TASK/CSN%20BOOTCAMP%20WEEK%208%20S3%20BUCKET%20NOT%20SECURED%20URL%20ENDPOINT.png)

# CLOUDFRONT DISTRIBUTION SETTINGS
![Cloudfront Distribution Settings](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week8/CSN%20BOOTCAMP%20WEEK%208%20TASK/CSN%20BOOTCAMP%20WEEK%208%20CLOUDFRONT%20DISTRIBUTION%20SETTINGS.png)

# CLOUDFRONT DEPLOYMENT STATUS
![Cloudfront Distribution Deploymet Status](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week8/CSN%20BOOTCAMP%20WEEK%208%20TASK/CSN%20BOOTCAMP%20WEEK%208%20CLOUDFRONT%20DISTRIUTION%20STATUS%20ENABLED.png)

# LIVE WEBSITE AS ACCESSED THROUGH CLOUDFRONT DOMAIN
![Cloudfront Domain Live Website](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week8/CSN%20BOOTCAMP%20WEEK%208%20TASK/CSN%20BOOTCAMP%20WEEK%208%20CLOUDFRONT%20DOMAIN%20LIVE%20WEBSITE.png)


## LESSONS LEARNED
- I learned how to host static websites using AWS S3. 
- I understood how CloudFront improves content delivery and adds a layer of security . 
- I gained experience configuring bucket policies and working with AWS edge services.
