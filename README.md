# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/dcd4402f-5ad1-4ffc-8116-e8309f414d0a)

Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 ![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/5e3506c7-5a8f-4840-9b86-7c1b7d944019)

Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/e0c9d542-67e8-4dbe-a201-eac94116d229)

Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/3f4b4e27-f253-4369-9db7-e670619b8bef)

Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).


Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/6ca86ee9-9bff-4bfc-9dc0-d9c141ad8ed0)

Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse.
Step 4: Carefully select your RESTful resource (web service) and click OK.
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/d305728e-79c6-4238-abe6-803cb98b35c2)
 
Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/4085cdd4-8007-4857-9699-d4af7fe6bdc8)

Step 6: An editing tab will open. Alter getHtml() method with the following.
 ![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/0af76755-e9c8-4947-a5f6-d0747b431cca)
 
Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/0aa5abf0-f902-4d09-83b2-bd9b5cb29b04)

Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 ![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/4978afda-b98f-4280-85f0-bd48a1c729c2)

Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/1b8ec024-0df4-4706-b863-6d31ceb3a99c)


Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
![image](https://github.com/nithish143257/Ex-04_RESTful_Web_Services/assets/113762839/e220bba8-4ce7-4376-80f7-46ff6c0c840b)
 
 
Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
