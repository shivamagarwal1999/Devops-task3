# Devops-task3

Problem Statement :

Create a container image that has jenkins,kubernetes installed using Dockerfile. When we launch this image it should automatically start the jenkins service in the container.
Create a chain of jobs which will help to fetch source code, start Kubernetes service and launch container with deployment and pvc , test service, notify the status and in case of failure it will have capability to launch new environment in less that a minute or may be in just 1 second.

Task Description :

1. Create container image that has Jenkins and kubernetes installed using Dockerfile.

2. When we launch this image, it should automatically starts Jenkins service in the container.

3. Create a job chain of job1, job2, job3 and job4 using build pipeline plugin in Jenkins .

4. Job1 : Pull the GitHub repository automatically when some developers push code or file  to Github.

5. Job2 : 

  1. By looking at the code or program file, Jenkins should automatically start the respective language interpreter installed image container ( ex. If code is of PHP, then Jenkins should start the container that has PHP already installed ) to deploy code on top of Kubernetes (use Kubernetes resources like Pods, ReplicaSet, Deployment, PVC and Service).

2. Expose your pod so that testing team could perform the testing on the pod

  3. Make the data to remain persistent ( If server collects some data like logs, other user information )

6. Job3 : Test your app if it is working or not.

7. Job4 : if app is not working , then send email to developer with error messages and redeploy the application after code is being edited by the developer
