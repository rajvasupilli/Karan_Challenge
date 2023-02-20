
## Prerequisites: In order to make use of the role, you will have to address the below prequisites

1. Install Ansible
2. Install Python3
   ``` sudo apt install python3-pip ```   
3. Install Boto3
   ``` sudo pip3 install boto3 ```
4. Install AWS CLI verison 2 and configure the aws credentials

### The folder named nginx-autoscaling contains the Ansible Role configuration which will provision the below resources in AWS:

   1. EC2 Key Pair
   2. EC2 Security Group
   3. EC2 Launch Configuration
   4. Auto Scaling Group
   
### Run the ansible playbook install-role.yml to install the ansible role. 
  
 ansible-playbook install-role.yml
 
## At the end of the execution give it sometime until the EC2 instances transitions into the Running state.
 
 Copy the "Public IPv4 DNS" of the EC2 Instance created via the Auto Scaling Group and paste it in the browser as below, to access the service.
 
 https://ec2-3-238-12-64.compute-1.amazonaws.com/ 


## Note: If you run into the error "botocore.exceptions.NoCredentialsError: Unable to locate credentials, apply the below fix.

      Store the AWS Credentials in the file /etc/boto.cfg as below.
      [Credentials]
      aws_access_key_id = AKIARD3FB6N4UCXI67NM
      aws_secret_access_key = 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
      
      An Ubuntu VM was used to test the Ansible role


