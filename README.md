Deployment Validation Steps
1. Login to Terraform Executor Instance
Login to console --> ec2 --> search for instance i-0559e268aa27aee3f --> connect


2. Check Terraform, Docker, kubectl, eksctl, and Git Installation
terraform -help
docker --version
kubectl version --client
eksctl version
git --version

3. Navigate to EC2 Demo Terraform Project
cd /home/ec2-user/ec2-demo/AWSEngagementReady
terraform show
Open the public IP output in the browser:
http://<public-ip>


4. Navigate to Modular Website Deployment
cd /home/ec2-user/module-websitedemo/AER-ModularWebsite/space-invaders-website
terraform show
Open the Load Balancer DNS name output in the browser:
http://<load-balancer-dns-name>



5. Git Repositories
EC2 Demo Project:
git clone https://github.com/Shreyas-Ravath/AWSEngagementReady.git
Modular Website Project:
git clone https://github.com/Shreyas-Ravath/AER-ModularWebsite.git
