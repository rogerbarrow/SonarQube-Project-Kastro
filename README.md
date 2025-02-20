1. Sonar Qube Introduction
2. Open-source plat form
3. Help static code analysis and code quality management 
4. Analyzes source code for bugs, Vulnerabilties, code smells, Code duplication 

Step 1. Launch EC2 instance 

![[Pasted image 20250219153140.png]]
step 2. SSH into the instance 

![[Pasted image 20250219155549.png]]

run the sudo apt update

![[Pasted image 20250219160238.png]]

Next lets Install Java
![[Pasted image 20250219160831.png]]

Next Install Jenkins
```bash
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins -y
```

Next open Port 8080

![[Pasted image 20250219164630.png]]
next login to Jenkins

![[Pasted image 20250219165054.png]]
next Lets Install Docker 
![[Pasted image 20250219165835.png]]

Instal Sonarqube

```bash
Step 5: SonarQube Setup
# Lets setup sonar server using Docker (this is the simplest way)
$ sudo apt install docker.io

#Lets give permissions to run docker
$ sudo chmod 666 /var/run/docker.sock

#Lets run docker commands to install SonarQube
$ docker run -d --name sonarqube -p 9000:9000 sonarqube:lts-community

$ docker ps

```

Run docker images to verify sonarqube is setup
![[Pasted image 20250219172613.png]]

Next open Port 9000 to access sonar qube

![[Pasted image 20250219173820.png]]

Next install jenkins Plugin

![[Pasted image 20250219180051.png]]
