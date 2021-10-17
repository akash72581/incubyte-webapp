# incubyte-webapp

#prerequisites:
1)aws EC2-instance as a deployment server.
2)centos act as a developer machine as well as jenkins server(automation server).
3)Dokcer on both machine(aws and centos)
4)github repository

#steps:
1)install docker,java,jenkins on centos machine.
2)create one repository on git hub 
3)developer clone that repository on his own machine and push the code on that particular repo.
4)configure jenkins for 3 jobs(fetch-code,build-image,execute-container).
5)make one ec2-instance on aws as a deploymant server(production server).

#configure pipeline using jenkins:

job1:fetch-code -->job2:build-image -->job3:execute-container 
