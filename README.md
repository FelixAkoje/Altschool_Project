# Altschool_Project

Project Title: Provision a linux server with a simple HTML page.

Project Description:

Provisioning of the server on AWS: An EC2 instance is a virtual server in the AWS cloud. To provision the server, i had to locate EC2 by searching it on the left part of the amazon dasboard. Then i head to instance and launch instance. It brought a page for me to configure and install an operating system of my choice. The following are the steps i followed to set it up:
Name the server
choose Ubuntu linux distro from the list of Operating systems available.
Choose my preferred Amazon Machine Image.
Choose my Preferred architecture of 64 bit.
Choose an instance type.
Created a new key-pair.
Created a new security group, under the inbound rule, i HTTP traffic on port 80 from anywhere. I also configured SSH through port 22 to allow me manage the server from anywhere.
Web Server Setup: After i SSH into the server, i had to make myself the root user using "sudo su". I then updated the server using "apt update". After which i installed Apache web server using "apt install apache2"

HTML page deployment: I created a simple HTML page and did simple styling with CSS.

Deploing the html web application on the server:
I change directory to /var/www/html using the command cd '/var/www/html'
From the html directory, i had to download my web files from my git repository using wget command. the cammand and the part is:  "wget https://github.com/FelixAkoje/Altschool_Project/archive/refs/heads/main.zip"

After downloading the files, i had to unzip the file using the command "unzip main.zip"

After unzipping, i copied the content of the unzipped folder to the html directory using the command "cp -r Altschool_Project-main/* /var/www/html/"

I restarted my apache and confirm if it's running using my public Ip address from my EC2 instance which is: 18.212.29.215
