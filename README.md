# AWS Security Group Resource Finder


Surprisingly, AWS doesn’t provide a direct way to see which resources are associated with each security group. To address this, I created a BASH script that loops through all security groups within a specific VPC and lists the attached resources. (You can easily modify it to loop across all VPCs in a region.)
Currently, the script identifies associations with EC2 instances, ENIs, RDS instances, and Load Balancers. While other AWS services can also be linked to security groups, I focused on the ones most relevant to my use case, which I believe are also the most commonly used.

In order to make use of the script please make sure you have aws-cli configured.
More about aws-cli can be found here = https://aws.amazon.com/cli/ 



# Using the script
<br/>

**Make the script executable**
````
chmod +x sg-resource-finder.sh
````
<br/>

**Run the script**
````
sh sg-resource-finder.sh
````
