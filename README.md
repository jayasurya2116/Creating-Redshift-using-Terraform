# Creating-Redshift-using-Terraform
Description:
Redshift is expensive to run, so I created this GitHub with the sole intention of having a handy way to create and destroy a terraform cluster.

Step 1:
We will use the Terraform snippet to create a Redshift cluster. We will also hold our newly created Redshift secrets inside of SecretsManager so we can access the cluster later.

file name: main.tf

Step 2:

terraform installed locally with your AWS credentials configured.

Follow following steps

1) Install AWS CLI
 https://awscli.amazonaws.com/AWSCLIV2.msi (64 bit for windows)

2) Check the version to verify for correct installation
aws --version
aws-cli/2.13.21 Python/3.11.5 Windows/10 exe/AMD64 prompt/off

3) Access
   Create Used group with required access from aws and download access key
   
4) AWS CLI Configiration
cmd: aws configure
AWS Access Key ID [None]: 
AWS Secret Access Key [None]: 
Default region name [None]: 
Default output format [None]: json

5) Terraform 
Make sure terraform is installed

Step 3:

terraform init
terraform plan
terraform apply

Step 4:

Redshift pricing starts in the the region of $219/month, so always make sure you either pause or destroy the cluser when you no longer need it.
terraform Destroy
