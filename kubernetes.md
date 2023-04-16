https://unofficial-kubernetes.readthedocs.io/en/latest/
https://training.play-with-kubernetes.com/

https://ranchermanager.docs.rancher.com/v2.5/pages-for-subheaders/rancher-on-a-single-node-with-docker

local kubernetes 1 node cluster with rancher 
docker run -d --restart=unless-stopped -p 80:80 -p 443:443 --privileged rancher/rancher:latest

go to the browser and enter "localhost:80"  then follow instructions to get the password to enter into rancher

you don't have the grep command in windows so remove the grep item and see the logs for  bootstrap password.

![kubernetes-part1.jpg](/.attachments/kubernetes-part1-d75b06ad-04a3-493d-9df3-7ba8700bbdd9.jpg)