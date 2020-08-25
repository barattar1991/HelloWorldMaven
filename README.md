# Description

### This repository is for the [Build a Java app with Maven](https://www.jenkins.io/doc/tutorials/build-a-java-app-with-maven/) tutorial in the [Jenkins User Documentation](https://www.jenkins.io/doc/) and  [Docker User Documentation](https://docs.docker.com/get-started/overview/).
### The repository contains a simple Java application which outputs the string "Hello world!" and is accompanied by a couple of unit tests to check that the main application works as expected.
### I worked on AWS Cloud, Created ec2 instance, OS- linux ubuntu.
### Installing Docker with the script requires.
### use the commands:
### curl -fsSL https://get.docker.com -o get-docker.sh
### sudo sh get-docker.sh
### docker version

<a href="https://ibb.co/kcgM27V"><img src="https://i.ibb.co/bdg750j/1.png" alt="1" border="0"></a>

# Jenkins Continuous Integration and Delivery server.
### Jenkins- an open source automation server which enables developers around the world to reliably build, test, and deploy their software.
### use the command:
### docker pull jenkins/Jenkins
### git pull command is used to fetch and download content from a remote repository and immediately update the local repository to match that content.
### Official Jenkins Docker Image
### use the command:
### Docker images
### The command will show the list of images:

<a href="https://imgbb.com/"><img src="https://i.ibb.co/PGNHYV6/2.png" alt="2" border="0"></a>

### Local volume for jenkins workspace folder and Web Ui Accessible on port 11000.
### use the command:
### docker run -d -v jenkins_home:/var/jenkins_home -p 11000:8080 -p 50000:50000 jenkins/jenkins:lts
### Explain about the options:
### Docker run -d  - Run container in background and print container ID.
### Docker run -v  - Bind mount a volume.

<a href="https://ibb.co/8KrGXgc"><img src="https://i.ibb.co/w0S8Yhs/3.png" alt="3" border="0"></a>
<a href="https://ibb.co/0f7P6HT"><img src="https://i.ibb.co/D7J3v0h/4.png" alt="4" border="0"></a>

### Connect the Container with root user and use bash shell in the container.
### use the command:
### sudo docker exec -u root -it 587ef54131d8 /bin/bash
### use the command:
### cat /var/jenkins_home/secrets/initialAdminPassword
### to get password-login to jenkins

<a href="https://ibb.co/52kYWXT"><img src="https://i.ibb.co/vDhsxC1/5.png" alt="5" border="0"></a><br /><a target='_blank' href='https://geojsonlint.com/'>json verifier</a><br />


### Install sudo in docker container follow commands(Optional to use sudo):
### use the commands:
### apt-get update
### apt-get -y install sudo
### Install Maven on the container:
### use the commands:
### sudo apt install maven – install maven
### mvn -version – check version of mvn
### Choose Manage Jenkins and choose Global Tool Configuration.
### Configure Maven in Jenkins settings:

<a href="https://imgbb.com/"><img src="https://i.ibb.co/Qn1jWvQ/6.png" alt="6" border="0"></a>

<a href="https://ibb.co/2n5CZW9"><img src="https://i.ibb.co/bW7CbQ0/7.png" alt="7" border="0"></a>

### Fork this Repo:

<a href="https://ibb.co/Fxdx3pH"><img src="https://i.ibb.co/tm1mKRL/8.png" alt="8" border="0"></a>
<a href="https://imgbb.com/"><img src="https://i.ibb.co/80H7GPn/9.png" alt="9" border="0"></a>
<a href="https://imgbb.com/"><img src="https://i.ibb.co/4fk8Wcp/10.png" alt="10" border="0"></a>

### Install plugins on jenkins:
[Workspace Cleanup Plugin](https://plugins.jenkins.io/ws-cleanup/), [Pipeline: GitHub Groovy Libraries](https://plugins.jenkins.io/pipeline-github-lib/), [Pipeline Maven Integration Plugin](https://plugins.jenkins.io/pipeline-maven/), [Pipeline](https://plugins.jenkins.io/workflow-aggregator/), [Oracle Java SE Development Kit Installer Plugin](https://plugins.jenkins.io/jdk-tool/), [Maven Integration plugin](https://plugins.jenkins.io/maven-plugin/), [GitHub plugin](https://plugins.jenkins.io/github/), [Docker Pipeline](https://plugins.jenkins.io/docker-workflow/), [Command Agent Launcher Plugin](https://plugins.jenkins.io/command-launcher/), [bouncycastle API Plugin](https://plugins.jenkins.io/bouncycastle-api/).

### Build a Pipeline-Click New item and give it name and then choose Pipeline.

[https://www.jenkins.io/doc/book/pipeline/getting-started/](https://www.jenkins.io/doc/book/pipeline/getting-started/)

[https://www.jenkins.io/doc/pipeline/steps/pipeline-utility-steps/](https://www.jenkins.io/doc/pipeline/steps/pipeline-utility-steps/)

<a href="https://ibb.co/68YsZtN"><img src="https://i.ibb.co/PMxCYWt/11.png" alt="11" border="0"></a>

<a href="https://ibb.co/tsb4f3H"><img src="https://i.ibb.co/ncDb2Rw/12.png" alt="12" border="0"></a>

<a href="https://ibb.co/z7J1HHd"><img src="https://i.ibb.co/qW5zFF6/13.png" alt="13" border="0"></a>

<a href="https://ibb.co/sQnTKsG"><img src="https://i.ibb.co/Np509WP/14.png" alt="14" border="0"></a>

<a href="https://imgbb.com/"><img src="https://i.ibb.co/VBqyRY3/15.png" alt="15" border="0"></a>

<a href="https://imgbb.com/"><img src="https://i.ibb.co/Lpg9df2/16.png" alt="16" border="0"></a>

<a href="https://ibb.co/QbgM0mZ"><img src="https://i.ibb.co/Vj1T6Bd/17.png" alt="17" border="0"></a>

<a href="https://ibb.co/C28X4Yv"><img src="https://i.ibb.co/vYqrfTm/18.png" alt="18" border="0"></a>

<a href="https://ibb.co/MSvggJn"><img src="https://i.ibb.co/B3pffYL/19.png" alt="19" border="0"></a>

<a href="https://ibb.co/f2sssb4"><img src="https://i.ibb.co/s2ZZZhy/20.png" alt="20" border="0"></a>

<a href="https://ibb.co/b7WjCGS"><img src="https://i.ibb.co/7bYxZ0w/21.png" alt="21" border="0"></a>
















