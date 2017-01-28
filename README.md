# infra-team-ci-cd

# our ci cd process using, docker, jenkins, ansible, and much much more.

At ironSource infra team, we are responsible for developing an automation framework to help test our various installers.
Deploying hundreads of microservices across different platforms, cloud providers and on-prem solutions can become a cumbersome
task. To alleviate the effort of supporting a growing, auto scalable architecture, we had to develop a flexible ci / cd process. One that is easily reused and one that its building blocks are easily replaced. 
The blog post will explain briefly the tools being used in the process. In the process we will write code in JavaScript, Ansible, Groovy (for declerative jenkins pipeline), and we will use tools like docker, jenkins, and aws as the cloud provider. No previuos knowledge is needed but if you want to deepen your knowledge, links will be provided at the end of the blog for further reading.
So without further ado, lets get started and explore the magical world of ci cd.

## Setting up jenkins

To follow along with the blog post you will need to setup a jenkins server.
You can use the provided jenkins-server.yml to spin up a dockerized jenkins server.
To minimize impact on your machine the only thing you need installed is docker. 
after we install docker, we will pull the latest image of ubuntu

```sh
docker pull ubuntu:16.04
```

from inside the demo folder we will use the following command to enter our docker container: 

```sh
docker run -it --rm --name $(basename `pwd`) -p 8000:8000 -v ${PWD}:/tmp -w /tmp ubuntu:16.04 bash
```

Essentialy what it does is delete the previuos container and enter the new container in the temp folder where all of our code resides. 

Now to install ansible in the container... Zigi: continue from here
