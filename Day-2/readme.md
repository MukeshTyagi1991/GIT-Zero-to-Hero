## Create S3 Bucket
  1. Create S3 Bucket with all public access
  2. Go to the S3 Bucket and then go to the properties tab to eanble the Static website hosting with below redirection rules

   
                    
    [
     {
        "Condition": {
            "KeyPrefixEquals": "home"
        },
        "Redirect": {
            "ReplaceKeyPrefixWith": "index.html"
        }
     }
    ]

  3. Click on the Bucket website endpoint and you will get permission issue       

<img width="1104" height="405" alt="image" src="https://github.com/user-attachments/assets/71d5058a-cbdb-43ef-9a6e-0333b3765118" />


<img width="817" height="336" alt="image" src="https://github.com/user-attachments/assets/41e3c5ca-f9ab-4e6f-a5a1-49755b19024c" />





  4. For this you need to give the permission so need to go to the permission tab and give the object read permission ( as per your requiremnet ) through bucket policy


          {
    "Version":"2012-10-17",		 	 	 
    "Statement": [{
        "Sid": "AllowGetObject",
        "Principal": {
            "AWS": "*"
        },
        "Effect": "Allow",
        "Action": "s3:GetObject",
        "Resource": "arn:aws:s3:::test-demo-bucket-d/*"
    }]
}


5.with the help of this permission, now you are able to reslove the permission error issue

<img width="1045" height="383" alt="image" src="https://github.com/user-attachments/assets/42b399be-7c7e-4d07-95e6-a75285b19865" />


6.Now the issue with that there is no index.html file that why we are facing this issue , to reslove this issue we need to create a index.html file and upload into the S3 bucket 

index.html

error.html 

7. Once you upload the index.html file and error.html file then you are bale to login the same URL without any issue 




## create IAM user







## create a EC2 instance and download the AWS CLI latest version on that particluar machine so that we can access the S3 bucket from instances 

configure the AWS through AWS configure command and give the AWS access key and id 

once everthing is done you can check the access through AWS s3 ls command

aws s3 ls
aws s3 cp s3://bucket name/ .






