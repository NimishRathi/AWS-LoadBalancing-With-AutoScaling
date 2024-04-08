# AWS-LoadBalancing-With-AutoScaling
### AWS Auto Scaling and Load Balancer Deployment
This repository contains the documentation for deploying two websites using AWS Auto Scaling and a load balancer via the AWS Management Console.
This deployment utilizes AWS services to ensure high availability and scalability of your websites. AWS Auto Scaling automatically adjusts the number of instances in response to demand, while the load balancer evenly distributes incoming traffic to these instances.
![GitHub Logo](https://github.com/NimishRathi/AWS-LoadBalancing-With-AutoScaling/blob/313ab7f14a7f46eca3a9828557620f5493050b14/Screenshot%202024-04-03%20013334.png)
use the launch template so that the scaling instances will be of desired template 
### Deployment Steps
Follow these steps to deploy your websites using AWS Auto Scaling and a load balancer:

### Create Launch Configuration:
Navigate to the EC2 service.
Click on "Launch Configurations" under "Auto Scaling" in the sidebar menu.
Click "Create launch configuration" and follow the prompts to configure your launch configuration, including selecting the appropriate Amazon Machine Image (AMI), instance type, security groups, etc.
ssh into the machines and edit the httpd[Webserver] configuration.


### Set Up Auto Scaling Group:
After creating the launch configuration, navigate to "Auto Scaling Groups" under "Auto Scaling" in the sidebar menu.
Click "Create Auto Scaling group" and follow the prompts to configure your auto scaling group, including setting the desired capacity, scaling policies, etc.
![GitHub Logo](https://github.com/NimishRathi/AWS-LoadBalancing-With-AutoScaling/blob/313ab7f14a7f46eca3a9828557620f5493050b14/Screenshot%202024-04-03%20013417.png)
![GitHub Logo](https://github.com/NimishRathi/AWS-LoadBalancing-With-AutoScaling/blob/313ab7f14a7f46eca3a9828557620f5493050b14/Screenshot%202024-04-03%20013351.png)


### Register Instances with Load Balancer:
After creating the load balancer, navigate to its details page.
![GitHub Logo](https://github.com/NimishRathi/AWS-LoadBalancing-With-AutoScaling/blob/313ab7f14a7f46eca3a9828557620f5493050b14/Screenshot%202024-04-03%20013406.png)
Under "Instances" tab, click "Edit instances" and select the instances you want to register with the load balancer.

### Real-world Example: E-Commerce Website
Imagine you're deploying an e-commerce website using AWS Autoscaling and Load Balancer services. During peak shopping seasons, such as Black Friday, your website experiences a surge in traffic. With Autoscaling, AWS automatically adds more instances to handle the increased load, ensuring your website stays responsive and available. The Load Balancer evenly distributes incoming traffic across these instances, optimizing performance and reliability for your shoppers. After the shopping season ends, Autoscaling scales down the instances to save costs, allowing your infrastructure to adapt to varying demand seamlessly.




