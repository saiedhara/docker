# docker


4 How to install Docker in AWS EC2 Insatance | AWS EC2 Tutorial | RAJASEKHAR REDDY


Install Docker on AMI instance
=================================
1. Update the installed packages and package cache on your instance.

sudo yum update -y

2. Install the most recent Docker.

sudo yum install docker -y

3. Start the Docker service.

sudo service docker start
sudo service docker status

4. Add the ec2-user to the docker group so you can execute Docker commands without using sudo.

sudo usermod -a -G docker ec2-user

5. Verify that the ec2-user can run Docker commands without sudo.

docker  --version or docker info

6.restart ec2 instance

sudo reboot
