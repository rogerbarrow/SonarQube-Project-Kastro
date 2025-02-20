How to Get Started with SonarQube
Create a EC2 instance


![image](https://github.com/user-attachments/assets/0f08b199-8837-435c-b37d-71c79de23ebc)


SSH into your Instance

![image](https://github.com/user-attachments/assets/698d8cf3-ad1e-4098-8d0c-dbe5441bc73e)


Run the sudo apt update

![image](https://github.com/user-attachments/assets/e049c488-142c-4019-9ada-aa06d61a2cd4)

Next Install Java

![image](https://github.com/user-attachments/assets/b8dbf8d8-026b-4146-aa3d-1dc99eb9653b)

Verify Java is install


Next Install Jenkins
![image](https://github.com/user-attachments/assets/6a3a065c-5b07-484c-ad90-b950b10478c7)


Next Open Port :8080 in your Inbound Security Group

![image](https://github.com/user-attachments/assets/e50c4a93-e6d1-4a35-aafd-8acf67280b22)


Next install Docker

![image](https://github.com/user-attachments/assets/50a26cc8-4a1f-470e-8356-8dd2aaf9d4f7)

Next install SonarQube

![image](https://github.com/user-attachments/assets/5350fada-fbb0-481a-801a-c7b46aae063e)

Run docker images to verify the sonarqube is setup
![image](https://github.com/user-attachments/assets/8648d46d-9a0a-4db3-8798-851140bb4619)


next open Port 9000: so we acess sonarqube

![image](https://github.com/user-attachments/assets/efb397dd-4198-4941-930c-d09928673249)


next install Jenkins plugin

![image](https://github.com/user-attachments/assets/44f74b1d-d9fc-4751-9eec-ed5d234f415e)

install sonarqube plugins

![image](https://github.com/user-attachments/assets/3c31ece5-d599-4f64-a363-f29d9c1396b7)

Add sonar qube access token to Jenkins

![image](https://github.com/user-attachments/assets/123362b7-361c-4d43-99ec-2e306ad24312)

Add Sonar-server URL into Jenkins

![image](https://github.com/user-attachments/assets/b83e422c-a4d7-45f3-b403-e8f2fbe98ebe)

next we update the Jenkins grovvy

![image](https://github.com/user-attachments/assets/0726f497-c468-44c4-b550-45812e45773f)


lets run a Build

![image](https://github.com/user-attachments/assets/e2adf668-ae8c-4b66-b236-cf767c0a1e52)


Review your code via Sonarqube


![image](https://github.com/user-attachments/assets/a9cc4d62-9df7-4d8e-afb7-1288313da083)

We can go to Docker Hub to verify that the image was push


![image](https://github.com/user-attachments/assets/45f04262-f490-4dab-9b24-2639d7efdfa5)

update the security group to the port on you application I was using Port 5555

![image](https://github.com/user-attachments/assets/ce4ab1dd-ef8a-4d82-aa33-165543d368b6)

Conclusion
SonarQube is a game-changer for software development, ensuring high-quality, secure, and maintainable code. By automating code reviews, enforcing security standards, and reducing technical debt, it empowers developers and DevOps teams to build better software faster and with confidence.


