# jenkins-tutorial
2022-06-20 ~ 2022-06-21

sudo apt install ca-certificates
sudo apt install openjdk-11-jdk

wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
sudo apt update

sudo apt install jenkins

