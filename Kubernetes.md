https://medium.com/@hiamitchaurasia/getting-started-with-minikube-on-windows-kubernetes-5da2049a7f5f

https://github.com/alijahnas/CKA-practice-exercises


https://dev.to/subodev/50-questions-for-ckad-and-cka-exam-3bjm

**kubernetes application deployment example:**
https://learn.microsoft.com/en-us/azure/aks/tutorial-kubernetes-prepare-app

https://ranchermanager.docs.rancher.com/v2.5/pages-for-subheaders/rancher-on-a-single-node-with-docker 



local kubernetes 1 node cluster with rancher
docker run -d --restart=unless-stopped -p 80:80 -p 443:443 --privileged rancher/rancher:latest

go to the browser and enter "localhost:80" then follow instructions to get the password to enter into rancher

you don't have the grep command in windows so remove the grep item and see the logs for bootstrap password.

![kubernetes-part1.jpg](/.attachments/kubernetes-part1-5eb111ac-7c06-47fc-a98b-233e0bfb3416.jpg)

