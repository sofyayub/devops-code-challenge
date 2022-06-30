# Overview
1) This code is made up of two parts. FrontEnd and Backend. Both the files are dockerized.

# Solution
1) The base code is present inside the folder named as "solution"
2) Inside "solution/frontend" folder, the Docker file is present.<br>
  2.1) The docker image can be build as "sudo docker build -t frontend-server ." <br>
  2.2) This creates the image named as "frontend-server".<br>
  2.3) Run the image by the command "sudo docker run -p 3000:3000 -d frontend-server"<br>
3) Inside "solution/frontend" folder, the Docker file is present.<br>
  3.1) The docker image can be build as "sudo docker build -t backend-server ."<br>
  3.2) This creates the image named as "backend-server".<br>
  3.3) Run the image by the command "sudo docker run -p 8080:8080 -d backend-server"<br>
4) Please note that the CORS Error will arise, which can be changed by modifying the file inside "backend" code inside the "CORS" location
5) All the code is cloned from the repo(This repo), which means that if any change happens, and if Steps(2) and (3) are repeated, then the code will have the latest changes. Thus the code will always run the latest code whenever the code is "run".
6) As of now, this is running on the ElasticIP (on EC2 instance) so it can be accessed as given below.
 

# URL Checks
1. FrontEnd: http://3.143.137.240:3000/
2. Backend : http://3.143.137.240:8080/

# Future Tentative Enhancements
1. These images can be saved to ECR/DockerHub
2. The Images can be then run on ECS/EKS
3. We Can also add the Pipeline(AWS Code Pipeline) for automatic deployments. Or we can also use Jenkins for the same.


You can contact me on : mmerima310@gmail.com
