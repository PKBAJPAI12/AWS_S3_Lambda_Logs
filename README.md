# AWS_S3_Lambda_Logs

### Created IAM Role LambdaBasicExecutionRole
![Screenshot (17)](https://github.com/user-attachments/assets/e27f4b54-7e53-49be-b236-4e0b6dc1bf97)

### Attach Policy for AWSLambdaBasicExecutionRole
![Screenshot (18)](https://github.com/user-attachments/assets/4416ca40-7045-4957-8a26-de31d0d8fa92)

### Created Bucket of Name aws-raw-data-bucket
![Screenshot (19)](https://github.com/user-attachments/assets/320a22cb-0424-4353-9939-473f818cfec7)

### Created Folder aws-data
![Screenshot (20)](https://github.com/user-attachments/assets/a08834c4-cd98-42f6-87ed-4bdfafc6d36b)

### No Object in aws-data folder
![Screenshot (21)](https://github.com/user-attachments/assets/f7c0b8ee-7964-4db1-9ddb-abb058599099)

### Created Lambda Function S3EventLambda with using existing IAM Role LambdaBasicExecutionRole
![Screenshot (23)](https://github.com/user-attachments/assets/703e6156-e6c4-473a-a345-f8a95af9c434)
![Screenshot (24)](https://github.com/user-attachments/assets/81d95ea6-0bc3-4999-ab6d-7c5214482154)

### Created Lambda Trigger of S3 Bucket for Event s3 Object Created with prefix and suffix
![Screenshot (25)](https://github.com/user-attachments/assets/a45473da-b2cb-44b8-881c-00386604ee0f)

### s3 file abc.txt is uploaded
![Screenshot (22)](https://github.com/user-attachments/assets/03bb2f59-8049-4919-b6ba-61469b60230d)

### Logs Group Created when s3 object file is uploaded and S3EventLambda is triggered
![Screenshot (26)](https://github.com/user-attachments/assets/4c448338-9e78-45de-93c4-51dd5bb3e714)

### Logs Group showing error is s3.GetObject because its not attached s3 read policy with role
![Screenshot (27)](https://github.com/user-attachments/assets/0dd39cd1-bf47-41a9-8bc2-4028ba79482b)

### Update IAM Role LambdaBasicExecutionRole with attached 1 more policy S3ReadOnlyAccess
![Screenshot (28)](https://github.com/user-attachments/assets/aa3a4592-5942-4e87-9c36-5bc074c860af)

### Again Uploaded s3 file abc.txt
![Screenshot (29)](https://github.com/user-attachments/assets/86bb7eef-44c4-403e-adfd-38aced350168)

### Now Logs Group showing  without any error and is able to read s3 properties because of S3ReadOnlyAccess policy
![Screenshot (30)](https://github.com/user-attachments/assets/f3ed3207-f5f4-46c2-8736-70616a8ff9ab)
