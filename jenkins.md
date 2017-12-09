# Steps for setting up jenkins:

* Started with creating EC2 instance on AWS
* Logged into AWS cli and updated Java
* Installed Jenkins
* Installed Docker and Git so everything can work together (AWS, Jenkins, Git and Docker)
* Created ssh key for the GitHub plugin on Jenkins
* Added the key to my GitHub keys
* Created Jenkinsfile and created Jenkins project/pipeline and verified that it ran all stages defined in the Jenkinsfile.

There might have been some minor fixes to get Jenkins working but nothing I can remember and if so it was a minor fix. For me the hard part for me was not to get Jenkins instance running but to make the tic-tac-toe project go through the pipeline as of now everything should be working (builds and runs the project, runs the tests, builds to Docker).

#### Link to Jenkins

[Click here to go Jenkins](http://ec2-18-216-6-111.us-east-2.compute.amazonaws.com:8080/) 

#### Link to Docker

[Click here to go to Docker](https://hub.docker.com/r/fridthjofur12/tic_tac_toe/)
