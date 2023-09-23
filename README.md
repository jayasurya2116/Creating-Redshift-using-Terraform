# Creating-Redshift-using-Terraform
Description:
Redshift is expensive to run, so I created this GitHub with the sole intention of having a handy way to create and destroy a terraform cluster.

Step 1:
We will use the following Terraform snippet to create a Redshift cluster. We will also hold our newly created Redshift secrets inside of SecretsManager so we can access the cluster later.

file name: main.tf

Step 2:

terraform installed locally with your AWS credentials configured.

Step 3:

terraform init
terraform plan
terraform apply

Step 4:

Redshift pricing starts in the the region of $219/month, so always make sure you either pause or destroy the cluser when you no longer need it.
terraform Destroy
