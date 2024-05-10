<h1>AWS Multi Instance Deployment With Docker Orchestration </h1>

<h2>Description</h2>


This project involved deploying three virtual machines (VMs) on AWS infrastructure. VM1 was provisioned via the AWS Console as a plain EC2 instance without any installed applications. VM2 and VM3 were deployed using a Python script and the Boto3 library, placing them into different subnets as specified. Each of VM2 and VM3 was configured to run three containerized applications using Docker: two NGINX webservers and one MongoDB instance. Additionally, security groups were created to enable specific communication patterns between the Admin's PC and the VMs, as well as between VM1, VM2, and VM3. This project showcases proficiency in cloud deployment, containerization, networking, and security management on AWS.

<br />
<br />
<br />
<h2>
<p align="center">
Main Diagram<br/>
 <br />
<img src="https://imgur.com/R8PGERP.png" height="40%" width="80%" alt="Disk Sanitization Steps"/></p>
<br /></h2>
<br />
<h2>Languages and Utilities Used</h2>

- <b>Python was utilized for scripting the deployment of VM2 and VM3 using the Boto3 library, enabling programmatic interaction with AWS services.</b>
- <b>Boto3 library facilitated programmatic interaction with AWS services, enabling the creation and management of EC2 instances.</b>
- <b>Docker was employed to containerize the applications on VM2 and VM3, providing a lightweight and scalable environment for running NGINX webservers and MongoDB containers.</b>

<h2>Environments Used </h2>

- <b>The project was executed within the AWS cloud environment, leveraging its infrastructure services to deploy and manage virtual machines.</b>
- <b>Linux-based operating systems, such as Amazon Linux,, were utilized for the EC2 instances to support Docker and other required software components.</b>

<h2>Program walk-through:</h2>

- Deployed VM1 using the AWS Console, and VM2 and VM3 using a Python script with the Boto3 library, ensuring placement in different subnets as specified in the provided network diagram.
- Configured user data scripts for each EC2 instance to meet specific requirements: VM1 initialized as a plain EC2 instance with no applications installed, while VM2 and VM3 were set up to run three containerized applications each, including two NGINX webservers and one MongoDB container.
- Created security groups to facilitate communication as outlined in the provided specifications and Table 1, enabling SSH access from the Admin's PC host to VM1, VM2, and VM3's public addresses, as well as HTTP access to specific ports on VM2 and VM3's containerized applications.
- Established rules within the security groups to allow HTTP communication between VM1 and the containerized applications on VM2 and VM3, as well as ICMP (ping) communication between VM1 and the private addresses of VM2 and VM3.
- Successfully tested and verified the achieved goals, ensuring seamless communication between the specified entities according to the project requirements and network diagram.





<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
