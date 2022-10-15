# Create-a-snapshot-of-the-EBS-volume-of-running-instance-using-CLI
Create a snapshot of the EBS volume of running instance, give description (This is my  Webserver) and tags (Key- Project, Value- Production)


aws ec2 create-snapshot --volume-id vol-08a42dd37363bbdfa --description "This is my Webserver" 

aws ec2 create-tags --resources snap-052c6bb9c65b8d11c --tags Key=Project,Value=Production

![image](https://user-images.githubusercontent.com/109040029/195967689-3235f88f-96df-48cb-baa9-dbdcedcc7a38.png)

![image](https://user-images.githubusercontent.com/109040029/195967709-ac120131-7f61-4030-8148-c249f4e719b3.png)

aws ec2 create-snapshot --volume-id vol-08a42dd37363bbdfa --description "This is my Webserver" 

aws ec2 create-tags --resources snap-052c6bb9c65b8d11c --tags Key=Project,Value=Production

![image](https://user-images.githubusercontent.com/109040029/195967724-96704d33-13a0-4719-961a-56e1215cc246.png)

To terminate the instance:
aws ec2 terminate-instances --instance-ids i-0b8c4d9af6873f57f
