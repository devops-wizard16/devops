# Jenkins Installation

To install Jenkins on Debian/Ubuntu systems, follow these steps:

```bash
sudo apt update
sudo apt install openjdk-17-jdk
java -version
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins
```
## script copied from 
``` bash
    https://www.jenkins.io/doc/book/installing/linux/#debianubuntu