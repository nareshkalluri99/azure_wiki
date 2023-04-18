# How to push Docker images to ACR 

**Step-1:** 

Make sure you are connected with correct azure subscription.

By using

**az account show** 

![Screenshot 2023-04-18 at 12.48.31 PM.png](/.attachments/Screenshot%202023-04-18%20at%2012.48.31%20PM-88105ad3-7f2f-4f14-852f-5822dd449dae.png)


**Step-2:** 

Connect / Login with the ACR.

By using

**az acr login --name prosandemoecr**

Here in the place of prosandemoecr you can place your respective container registry name.

![Screenshot 2023-04-18 at 12.50.55 PM.png](/.attachments/Screenshot%202023-04-18%20at%2012.50.55%20PM-e390d870-34dc-42e5-9915-62284521f91f.png)

**Step-3:** 

First make sure you already have the respecive image on docker readily to push into ACR.

If you dont have any image on docker. For example if you want to pull nginx image you can pull that image in docker by using

**docker pull nginx:latest**

**Step-4:**

once you have the image in docker. Now its time to build the tag which is used to push the image to ACR.

Here i'm taking my nginx image on docker.

By using

**docker tag nginx prosandemoecr.azurecr.io/nginx:v1**

Here 
nginx is my image on docker
prosandemoecr.azurecr.io is my ACR hostname.
nginx:v1 is i'm pushing the image with name nginx and tag v1

![Screenshot 2023-04-16 at 8.07.15 PM.png](/.attachments/Screenshot%202023-04-16%20at%208.07.15%20PM-66aafb20-d44a-4406-91ba-087a4f304bc2.png)

Now you can see the image pushed to ACR.

**Step-5:**

Now will go and check on ACR whether the image is pushed correctly or not.

![Screenshot 2023-04-16 at 8.04.01 PM.png](/.attachments/Screenshot%202023-04-16%20at%208.04.01%20PM-d80053e5-42e7-497c-bb15-39544568d69d.png)

If you see i have the image now with name nginx and tag v1 on ACR.



## Reference: 

https://jonnychipz.com/2021/02/22/create-and-push-a-docker-image-to-azure-container-registry/



