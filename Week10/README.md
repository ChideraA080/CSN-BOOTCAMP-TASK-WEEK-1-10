# DESCRIPTION OF WHAT I DID FOR WEEK 10


# S3 TO LAMBDA INTEGRATION

This project demonstrates how to set up an **AWS Lambda function** that automatically triggers when a new file is uploaded to an **Amazon S3 bucket**. The Lambda reads the event data and logs the bucket name and file name to **CloudWatch Logs**.


## WHAT I DID
- I created an S3 bucket named `chidera-week10-csn-task`.
- I created a Lambda function with Python 3.11 runtime.
- I added an **S3 trigger** for `ObjectCreated (All)` events.
- I used the following Lambda handler code to log upload details:

    ```python
    import json

    def lambda_handler(event, context):
        print("Received event: " + json.dumps(event))
        try:
            records = event.get("Records", [])
            for r in records:
                bucket = r["s3"]["bucket"]["name"]
                key = r["s3"]["object"]["key"]
                print(f"New object uploaded: s3://{bucket}/{key}")
        except Exception as e:
            print("Error parsing event:", str(e))
        return {
            "statusCode": 200,
            "body": json.dumps("OK")
        }
    ```
- I Uploaded a test file `test.txt` via S3 console to trigger Lambda.
- I Verified the execution in **CloudWatch Logs** — confirmed bucket and file name logged.

  ## DELIVERABLES
- **S3 Bucket**: `chidera-week10-csn-task`
- **Lambda Function**: `s3-upload-logger-week10` (Python 3.11 runtime)
- **S3 Event Trigger**: Configured for `ObjectCreated (All)` events.
- **CloudWatch Logging**: Captures and displays event details upon file upload.

  
## SCREENSHOTS

# S3 BUCKET CREATED FOR THE TASK
![S3 Bucket Created](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week10/CSN%20BOOTCAMP%20WEEK%2010%20TASK/CSN%20BOOTCAMP%20WEEK%2010%20BUCKET%20CREATED.png)

# BUCKET UPLOADED STATUS
![Bucket Upload Status](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week10/CSN%20BOOTCAMP%20WEEK%2010%20TASK/CSN%20WEEK%2010%20BUCKET%20UPLOAD%20STATUS.png)

# BUCKET TEST.TXT FILE UPLOADED TO TEST TRIGGER
![Bucket test.Txt file Uploaded Status](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week10/CSN%20BOOTCAMP%20WEEK%2010%20TASK/CSN%20BOOTCAMP%20WEEK%2010%20BUCKET%20TXT%20FILE%20UPLOADED.png)

# S3 BUCKET SHOWING EVENT TRIGGER CONNECTED TO MY LAMBDA FUNCTION
![S3 Trigger Connected to Lambda Function](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week10/CSN%20BOOTCAMP%20WEEK%2010%20TASK/CSN%20BOOTCAMP%20WEEK%2010%20WITH%20S3%20BUCKET%20TRIGGER%20CONNECTED%20TO%20MY%20LAMBDA%20FUNCTION.png)

# IAM ROLE CREATED FOR LAMBDA EXECUTION
![IAM Lambda Role  ](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week10/CSN%20BOOTCAMP%20WEEK%2010%20TASK/CSN%20BOOTCAMP%20WEEK%2010%20IAM%20ROLES%20CREATED.png)

# LAMBDA FUNCTION CREATED
![Lambda Function Created  ](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week10/CSN%20BOOTCAMP%20WEEK%2010%20TASK/CSN%20BOOTCAMP%20WEEK%2010%20LAMBDA%20FUNCTION%20CREATED.png)

# LAMBDA FUNCTION CODE USED(PYTHON 3.11 RUNTIME)
![Lambda Function Code Used](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week10/CSN%20BOOTCAMP%20WEEK%2010%20TASK/CSN%20BOOTCAMP%20WEEK%2010%20LAMBDA%20FUNCTION%20CODE%20USED.png)

# LAMBDA SETTINGS/TRIGGER
![Lambda Settings/Trigger](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week10/CSN%20BOOTCAMP%20WEEK%2010%20TASK/CSN%20BOOTCAMP%20WEEK%2010%20LAMBDA%20SETTINGS%20%20AND%20TRIGGER.png)

# CLOUDWATCH LOGS AND STREAMS
![CloudWatch Logs and Streams](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week10/CSN%20BOOTCAMP%20WEEK%2010%20TASK/CSN%20BOOTCAMP%20WEEK%2010%20CLOUDWATCH%20LOGS%20AND%20STREAMS.png)

# CLOUDWATCH LOGS SHOWING THAT THE FUNCTION WORKED
![CloudWatch Logs Showing Function Worked](https://github.com/ChideraA080/CSN-BOOTCAMP-TASK-WEEK-1-10/blob/main/Week10/CSN%20BOOTCAMP%20WEEK%2010%20TASK/CSN%20BOOTCAMP%20WEEK%2010%20CLOUDWATCH%20LOGS%20TO%20SHOW%20FUNCTION%20WORKED.png)

## LESSSONS LEARNED

- I learned how to connect S3 bucket events to a Lambda function.
- The importance of selecting the correct **event type** (`ObjectCreated (All)`) for catching uploads.
- How CloudWatch Logs show detailed Lambda execution results.
- How to troubleshoot missing log groups (trigger must first fire before logs appear).
  
  

