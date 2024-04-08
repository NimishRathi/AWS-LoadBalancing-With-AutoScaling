# AWS-LoadBalancing-With-AutoScaling
### AWS Auto Scaling and Load Balancer Deployment
This repository contains the documentation for deploying two websites using AWS Auto Scaling and a load balancer via the AWS Management Console.
This deployment utilizes AWS services to ensure high availability and scalability of your websites. AWS Auto Scaling automatically adjusts the number of instances in response to demand, while the load balancer evenly distributes incoming traffic to these instances.
### Deployment Steps
Follow these steps to deploy your websites using AWS Auto Scaling and a load balancer:

### Create Launch Configuration:
Navigate to the EC2 service.
Click on "Launch Configurations" under "Auto Scaling" in the sidebar menu.
Click "Create launch configuration" and follow the prompts to configure your launch configuration, including selecting the appropriate Amazon Machine Image (AMI), instance type, security groups, etc.
ssh into the machines and edit the httpd[Webserver] configuration.
![GitHub Logo]()


### Set Up Auto Scaling Group:
After creating the launch configuration, navigate to "Auto Scaling Groups" under "Auto Scaling" in the sidebar menu.
Click "Create Auto Scaling group" and follow the prompts to configure your auto scaling group, including setting the desired capacity, scaling policies, etc.

### Register Instances with Load Balancer:
After creating the load balancer, navigate to its details page.
Under "Instances" tab, click "Edit instances" and select the instances you want to register with the load balancer.



