# Transferring-Files-Across-AWS-S3-Buckets-in-Different-AWS-Accounts-Using-python-Scripting
Introduction:
This task is to Transferring Files Across AWS S3 Buckets in Different AWS Accounts Using AWS SDK python Script.
S3 is an object storage service that offers industry-leading scalability, data availability, security, and performance by Amazon.
In this Task, 2 AWS accounts are Included with their access and secret key.

Steps:
Case-1:
Firstly, log in to aws accounts (both accounts) and create the access and secret key and save the file in local repository. We conclude these accounts by names as Account-A and Account-B.
In assume that account-A is source account. Next, Go to S3 console and create a bucket with respected name (In this case, The bucket name is “test1s3source”) with bucket versioning enabling in it and create it.
 Next, Select the bucket and go to the permissions tab. In the permissions tab, go to the Access control list (ACL) and select the edit.
 After selecting, go to the Access for other AWS accounts section. Add the “Canonical user ID“of the Account-B and mark the all check marks ”read and write for ACL and Objects” and save it.
 .
Now repeat the same progress to the destination account (Account-B) create a bucket with respected name (In this case, The bucket name is “test2s3destination”) 
Next in Account-A, S3 bucket upload a sample file in it for the transfer.
 
Case-2: -
In this case, Install Visual Code and add new text file (Python file) and install boto3 by terminal “pip install boto3”.
After installing, copy and paste the code which is uploaded from github. 
In the code, define the region_name, aws_access_key_id, aws_secret_access_key,  source_bucket name  and destination_bucket name.
Now run the code. 
You can see the output printed as “File transfer complete.”
 
And the file is successfully transferred from one AWS account to AWS another account by Python script.
