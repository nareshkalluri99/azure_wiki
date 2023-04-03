# **Task-1:**

**Created an Docker account and logged on to my docker desktop.**

![Screenshot 2023-04-03 at 10.59.18 AM.png](/.attachments/Screenshot%202023-04-03%20at%2010.59.18%20AM-82f7a54b-ad53-4865-b118-d8b5a55b5789.png)

![Screenshot 2023-04-03 at 11.01.13 AM.png](/.attachments/Screenshot%202023-04-03%20at%2011.01.13%20AM-e5c6e2a8-2f3b-4a9a-a7d8-1dcbbf038a06.png)

**Pulled the image alpine:latest** 

docker pull alpine:latest 

**created a tag with my name for the existing image alpine to push the image to my registry**

docker tag alpine:latest nareshkalluri9/workspace alpine:naresh

**Pushed the image with my updated tag to the registry**

docker push nareshkalluri9/workspace:naresh

![Screenshot 2023-04-03 at 11.07.43 AM.png](/.attachments/Screenshot%202023-04-03%20at%2011.07.43%20AM-c1fbefd4-52b3-49de-99fa-289e5814e13c.png)


# Task-2:

**Copied the files from the feature_docker branch to my branch naresh_20230312.**

![Screenshot 2023-04-03 at 11.09.39 AM.png](/.attachments/Screenshot%202023-04-03%20at%2011.09.39%20AM-9899e687-409e-4e68-9530-2a7d69a6a189.png)

# Task-3: 

**Pulled the latest centos image** 

docker pull centos:latest

**Executed the image** 

docker run -t -d centos sh

It gives me the id 

2a681999c2837c35223142830d02f82daf77c73a9735c456b11cb2b420534c13

Now i executed the image 

docker exec -it 2a681999c2837c35223142830d02f82daf77c73a9735c456b11cb2b420534c13 sh 

**Perfomed the operation ls -ltr**

![Screenshot 2023-04-03 at 9.44.33 AM.png](/.attachments/Screenshot%202023-04-03%20at%209.44.33%20AM-ec83cd34-ee27-4a06-86bc-ec578bf87c5e.png)

# Task-4: 

**Created a volume storage named "naresh-storage"**

docker volume create naresh-storage

![Screenshot 2023-04-03 at 11.25.32 AM.png](/.attachments/Screenshot%202023-04-03%20at%2011.25.32%20AM-567303c6-c565-4e16-809b-8af660e6d1fd.png)

**Attached this storage to one container and created a file into it.**

![Screenshot 2023-04-03 at 11.27.42 AM.png](/.attachments/Screenshot%202023-04-03%20at%2011.27.42%20AM-5e44b021-8b1e-40c5-8371-3007560d79cc.png)

![Screenshot 2023-04-03 at 11.27.48 AM.png](/.attachments/Screenshot%202023-04-03%20at%2011.27.48%20AM-4a9b6bce-326c-45b8-a94d-1b325228e198.png)

**Now created another container with the same storage volume to check whether the file exits or not.** 

docker run -it -v naresh-storage:/shared-volume --name centos-volume2  centos

![Screenshot 2023-04-03 at 11.29.55 AM.png](/.attachments/Screenshot%202023-04-03%20at%2011.29.55%20AM-77d35271-f06d-4e61-b25d-739d837f969a.png)


# Task-5: 

**By using the cp command copied a demofile which i already created in desktop on local machine into the container.**

![Screenshot 2023-04-03 at 11.32.40 AM.png](/.attachments/Screenshot%202023-04-03%20at%2011.32.40%20AM-c3a879a0-3a44-4ac3-a222-bf58137bd3d9.png)

A demofile copied from local machine to the naresh directory in container.


**END OF THE TASKS**


