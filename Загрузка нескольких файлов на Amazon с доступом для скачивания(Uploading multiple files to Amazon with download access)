import boto3
from botocore.client import Config

ACCESS_KEY_ID = "*****"  // your Access Key
ACCESS_SECRET_KEY = '*****'  // your Secret Access Key
BUCKET_NAME = "your_bucket"
filename = ['your_file_1.exe', 'your_file_2.exe']
for x in filename:
    print(x)
    

    data = open(x, 'rb')

    s3 = boto3.resource('s3', aws_access_key_id=ACCESS_KEY_ID, aws_secret_access_key=ACCESS_SECRET_KEY, config=Config(region_name = 'your_region', signature_version="s3v4"))

    s3.Bucket(BUCKET_NAME).put_object(Key=x, Body=data,  ACL='public-read')

print("Done")
