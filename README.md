# infra-team-ci-cd

# our ci cd process using, docker, jenkins, ansible, and much much more.

At ironSource infra team, we are responsible for developing an automation framework to help test our various installers.
Deploying hundreads of microservices across different platforms, cloud providers and on-prem solutions can become a cumbersome
task. To alleviate the effort of supporting a growing, auto scalable architecture, we had to develop a flexible ci / cd process. One that is easily reused and one that its building blocks are easily replaced. 
The blog post will explain briefly the tools being used in the process. In the process we will write code in JavaScript, Ansible, Groovy (for declerative jenkins pipeline), and we will use tools like docker, jenkins, and aws as the cloud provider. No previuos knowledge is needed but if you want to deepen your knowledge, links will be provided at the end of the blog for further reading.
So without further ado, lets get started and explore the magical world of ci cd.


