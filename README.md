# jenkins-tutorial
2022-06-20 ~ 2022-06-21

sudo apt install ca-certificates
sudo apt install openjdk-11-jdk

wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
sudo apt update

sudo apt install jenkins

sudo systemctl start jenkins
sudo systemctl enable jenkins

sudo systemctl status jenkins

sudo cat /var/lib/jenkins/secrets/initialAdminPassword
5c3f576132204c17a3f4b7d454cddcb8

#80포트로 접속 후 GUI 설정

Click: Install suggested plugins

write profile

Manage Jenkins -> Manage Plugin
Plugins to install
 - Amazon ECR
 - Docker Pipeline

Check: Restart Jenkins when installation is complete ....

credentials save
Kind: AWS Credentials 
Scope: Global
ID: jenkins-aws-credentials
Access Key ID: your IAM user access key

test

