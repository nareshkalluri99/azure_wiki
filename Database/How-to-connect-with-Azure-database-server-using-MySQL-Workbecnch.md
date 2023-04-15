How to connect with Azure database server using MySQL Workbecnch

Step1: Log in to azure portal 
Step2: Go to search bar and search for azure database for My sql server


 ![image.png](/.attachments/image-69b85cc4-af26-4cfb-a6c4-cb6b766cff6f.png)

Step3: Click on the server it takes you to the overview page where you can find the server name server login id, status, configuration, location and all the basic required information about the server



![image.png](/.attachments/image-aeb7cc6b-5fff-46a9-938d-ff4cea92fb3f.png)

Step4:Go to chrome and open a new tab and search for MY ip address

![image.png](/.attachments/image-4788c03b-c72c-437a-95e8-57cc0248172c.png)

Step 5: come back to to the server overview page and Got to Networks scroll the page where you can Add your IP address to the server

![image.png](/.attachments/image-30bf917a-7a34-4041-8b26-e221844b265e.png)

Once you add the IP address save it 
Step6: Now go to your start menu in your system open MySQL Workbench 

![image.png](/.attachments/image-4a7e0e46-27be-4806-b7cd-e3bcf4224cad.png)
Step7: click on Add symbol 
![image.png](/.attachments/image-10813a8d-7e1b-4eb7-8073-7a816d26df4b.png)
Give the connection name same as the azure name 
Get the Host name from the server overview page 
Give the username: prosan
Click on store password: Venk@t123
![image.png](/.attachments/image-5246d716-8566-48a9-bc4f-87267a057e6f.png)
Click on Test connection it should give a pop that connection in successful 
After that click on OK 
![image.png](/.attachments/image-73d70d58-71f6-4123-b1ad-789342c5d6ab.png)
It shows all your connections
Click on prosan-demo-db-01 connection 
![image.png](/.attachments/image-03a96830-e938-4f77-9e24-e1782bf42291.png)
It takes you to the SQL editor when you can create database, schemas and insert tables 

