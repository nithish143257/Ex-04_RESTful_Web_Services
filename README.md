# Ex-04_RESTful_Web_Services
## Aim:
To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:
### Server side:
#### Step 1: 
Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
#### Step 2: 
Right-click on the project name and select New->RESTful Web Services from Patterns.

![image](https://github.com/MaheshS03/Ex-04_RESTful_Web_Services/assets/128498431/9487d6a0-b9ef-4079-a488-48bf9711fd1e)

#### Step 3:
A new window will appear. Select “Simple Root Resource” and click Next.
 
 ![image](https://github.com/MaheshS03/Ex-04_RESTful_Web_Services/assets/128498431/eeedcddb-9ac8-4cf0-864f-ae8356c0f50d)

#### Step 4:
In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/MaheshS03/Ex-04_RESTful_Web_Services/assets/128498431/ae01a92a-000b-4454-b816-f2bbf3c88b89)

#### Step 5: 
Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
#### Step 6:
Alter getHtml() method as shown below.
#### Step 7: 
Save your project, clean and build it. Deploy your project.
 
![image](https://github.com/MaheshS03/Ex-04_RESTful_Web_Services/assets/128498431/04360917-d8f0-4708-8223-5971795a528e)

#### Step 8:
To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).

### Client-Side:
#### Step 1: 
Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
#### Step 2:
Right-click on the project and select New->RESTful Java Client.

![image](https://github.com/MaheshS03/Ex-04_RESTful_Web_Services/assets/128498431/7b17dcab-48af-4d4a-b68f-2d0c0b88a0a8)

#### Step 3:
A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse.

#### Step 4:
Carefully select your RESTful resource (web service) and click OK.
 
 ![image](https://github.com/MaheshS03/Ex-04_RESTful_Web_Services/assets/128498431/b4c56033-7195-422b-acd3-ed338b3fc27e)

#### Step 5: 
Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/MaheshS03/Ex-04_RESTful_Web_Services/assets/128498431/344cc742-5b95-4d7f-a6ef-f181750991b0)

#### Step 6:
An editing tab will open. Alter getHtml() method with the following.
 
![image](https://github.com/MaheshS03/Ex-04_RESTful_Web_Services/assets/128498431/5cedb045-0c65-44fb-b581-a75ba58b43a2)

#### Step 7: 
Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![image](https://github.com/MaheshS03/Ex-04_RESTful_Web_Services/assets/128498431/17c761fa-0fdc-4b37-b59d-19ec22fadc3b)

#### Step 8: 
A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 
 ![image](https://github.com/MaheshS03/Ex-04_RESTful_Web_Services/assets/128498431/21d6ad7b-d2d6-4bd2-9b65-4193ef4fc6e1)

#### Step 9: 
Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
#### Step 10:
A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![image](https://github.com/MaheshS03/Ex-04_RESTful_Web_Services/assets/128498431/070bf360-824b-4ad0-be10-3e6ad3e28a94)

#### Step 11:
Save the project and build it.
#### Step 12:
Run the JSP file and you should see the output in a new browser window.
 
 ![image](https://github.com/MaheshS03/Ex-04_RESTful_Web_Services/assets/128498431/031a3725-b4be-4653-ab4b-b281bdb69bbf)

### Client-Side Remote Invocation:
#### Step 1: 
Follow steps 1-5 as in Section 2.2
#### Step 2: 
In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
#### Step 3: 
Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
