Project Title: Provision a linux server with a simple HTML page.

Project Description: 
 1. Provisioning of the server on AWS: An EC2 instance is a virtual server in the AWS cloud. To provision the server, i had to locate EC2 by searching it on the left part of the amazon dasboard. Then i head to instance and launch instance. It brought a page for me to configure and install an operating system of my choice. The following are the steps i followed to set it up:
     1. Name the server
     2. choose Ubuntu linux distro from the list of Operating systems available.
     3. Choose my preferred Amazon Machine Image.
     4. Choose my Preferred architecture of 64 bit.
     5. Choose an instance type.
     6. Created a new key-pair.
     7. Created a new security group, under the inbound rule, i HTTP traffic on port 80 from anywhere. I also configured SSH through port 22 to allow me manage the server from anywhere.

Web Server Setup: After i SSH into the server, i had to make myself the root user using "sudo su". I then updated the server using "apt update". After which i installed Apache web server using "apt install apache2"

HTML page deployment: I created a simple HTML page and did simple styling with CSS.

Deploing the html web application on the server:
 
 
 