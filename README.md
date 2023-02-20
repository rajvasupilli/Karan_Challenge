# Karan_Challenge

##Prerequisites: In order to make use of the role, you will have to address the below prequisites

1. Install Ansible
2. Install Python3
   ```sudo apt install python3-pip ```   
3. Install Boto3
   ```sudo pip3 install boto3```
4. Install AWS CLI verison 2 and configure the aws credentials

Note: If you run into the error "botocore.exceptions.NoCredentialsError: Unable to locate credentials, apply the below fix.

      Store the AWS Credentials in the file /etc/boto.cfg as below.
      [Credentials]
      aws_access_key_id = AKIARD3FB6N4UCXI67NM
      aws_secret_access_key = 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

An Ubuntu VM was used to test the Ansible role
