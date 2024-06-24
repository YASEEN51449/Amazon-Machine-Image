# Amazon-Machine-Image
********AMAZON MACHINE IMAGE*****

1.Create an Ec2 Instance(Linux)
2.Slect Amazon Linux Os
3.Create a Key Pair
4.Tokyo Region(Any)
5.Allow Https & Http
6.lanuch Instance
 
connect Linux instance--Linux-web
sudo su
yum update
--install web server
yum install httpd -y
cd /var/www/html/
cat >index.html
Hello world
cd 
systemctl start httpd   [service httpd start]
sysemctl enable httpd
syatemctl status https
check in web:copy and paste public ip in browser

mkdir test
ls
cd test
touch file1

on Linux instance go to action
--Image & Template
--Create Image
--Usually at production level Instance should be stop and after that we need to create image but at right we are creating instance while instance is running...
--Web-Image
--Desc:Wb-ser
--Create Image

Go to AMI---Pending it will take some time to create image from instance
give name to image --Linux_image
Linux-web---Terminate the instance
Go to AMI
Select--ACtion--Copy Ami
I can able to deploy in same region/also at different region too
Web-ohio
Us east-ohio
Go to ohio region check AMI at Ohio

go to Tokyo region where you created Launch Instance from AMI Web-1
key pair --new/existing
Launch instance

Now Again go to ohio and launch a instance from AMI
Name :ohio
create key pair
Launch instance
connect ec2 instance ---web
copy public ip
service httpd status
service httpd start
---if we migrate the server we need to start.
cd /var/www/html/
cat index.html








 


