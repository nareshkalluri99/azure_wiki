04/04 - CICD 


**Learned Topics in today's class:**

**Pipeline in Azure DevOps:**

- How to create CI (Continuous Intergration) Pipeline in Azure devops.

- What is an yaml file -> A file which contains the stages and jobs to be run in the pipeline.

- Got to know the each step of a yaml file like trigger, Pool, variables, stages, jobs and tasks. 

- Discussed how to overcome the azure pipeline parallelism issue and how to apply for that form.

- Learned how to connect the docker registry in the Azure devops and added my docker registry details into azure devops by using service connections.

![Screenshot 2023-04-05 at 2.59.12 PM.png](/.attachments/Screenshot%202023-04-05%20at%202.59.12%20PM-49f01fb2-4e07-47ad-a62f-18e5a75c2aa9.png)

# 
# 
**Jenkins:** 

- Created a Maven Pipeline.
- Learned how to install maven and jdk tools automatically by using Global Tool Configuration on Jenkins.
- Faced errors while running the pipeline in the build stage 

- Next copied the latest jdk download link by manually from the oracle cloud platform.
- By using the copied link with the commands wget and curl tried to install the latest jdk version in the Jenkins server but failed again.

- Downloaded the latest jdk file in the windows and copied that file into the Jenkins server by using WinSCP.

A WinSCP is a popular SFTP client and FTP client for Microsoft Windows! Copy file between a local computer and remote servers using FTP, FTPS, SCP, SFTP, ...

- Rebuilded the pipeline but this time we updated the jdk and maven paths in the pipeline.

- Still no use still stuck at the Error in the build stage.

Finally Ended our class with an unsolved error "/opt/apache-maven-3.8.8/bin/mvn: line 194: /opt/jdk1.8.0_202/bin/java: No such file or directory"


