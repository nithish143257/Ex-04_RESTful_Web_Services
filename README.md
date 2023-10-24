# Ex-04_RESTful_Web_Services
## Aim:
To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:
### Server side:
#### Step 1: 
Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
#### Step 2: 
Right-click on the project name and select New->RESTful Web Services from Patterns.

![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/9f4dc3f3-383c-4917-a40c-a64cb6a8152b)

#### Step 3:
A new window will appear. Select “Simple Root Resource” and click Next.
 
 ![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/be8348bf-d9eb-48e4-bf7a-ba5a5ed339ee)

#### Step 4:
In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.

![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/1d79d392-a772-4cfe-94d2-bce62751ee15)

#### Step 5: 
Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
#### Step 6:
Alter getHtml() method as shown below.
#### Step 7: 
Save your project, clean and build it. Deploy your project.
 
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/6ccc004e-aad1-402e-a540-a7b1a7951ea6)

#### Step 8:
To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).

### Client-Side:
#### Step 1: 
Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
#### Step 2:
Right-click on the project and select New->RESTful Java Client.

![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/6e7b96ff-6ae1-46a0-9341-55f71419993a)

#### Step 3:
A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse.

#### Step 4:
Carefully select your RESTful resource (web service) and click OK.
 
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/204de53f-4a41-4d20-b3d8-a6422d99fcdb)

#### Step 5: 
Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.

![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/0dd73880-f7d0-48ff-9382-1d1635072802)

#### Step 6:
An editing tab will open. Alter getHtml() method with the following.
 
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/27feb390-ca83-4d5e-ad49-3abae13a6850)

#### Step 7: 
Right-click on the Libraries folder under your project and select “Add JAR/Folder”.

![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/d5b85ede-3ec1-413b-9598-ade462638bd6)

#### Step 8: 
A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/49fa5c89-8074-4938-b013-c4e2bb52f974)

#### Step 9: 
Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
#### Step 10:
A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/60e3264c-092c-4e85-86dd-e1e269ed64e5)

#### Step 11:
Save the project and build it.
#### Step 12:
Run the JSP file and you should see the output in a new browser window.
 
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/8749464b-4baf-418c-9357-2ff46d434996)

### Client-Side Remote Invocation:
#### Step 1: 
Follow steps 1-5 as in Section 2.2
#### Step 2: 
In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
#### Step 3: 
Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
