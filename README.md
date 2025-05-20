![389206464-4d0066f0-975c-45e2-b66b-6b9f422905e2](https://github.com/user-attachments/assets/7a06b77d-a546-4353-a591-492c038f283d)# RESTful Web Services

## Aim
To create RESTful web services using both server-side and client-side implementations.

## Procedure

### Server-Side Implementation

1. **Create a New Java Web Project:**
   - Follow steps 1-5 from the SOAP-based Web Services section to set up a new Java Web Project.

2. **Create RESTful Web Services:**
   - Right-click on the project name and select `New` -> `RESTful Web Services from Patterns`.

     ![389206300-4c246ecc-e1d7-45d1-970a-854dcdc28736](https://github.com/user-attachments/assets/5eca2df7-0d50-473a-9202-561f6a180fe7)


3. **Configure Resource:**
   - In the new window, select `Simple Root Resource` and click `Next`.
   - Provide a Resource Package name and choose `MIME Type` as `text/html`. Click `Finish`.

     ![389206329-55fd4817-d869-4b4e-94ac-457c4a9bd390](https://github.com/user-attachments/assets/8de7390a-2b66-4037-b075-369f6f083d73)


4. **Edit Resource:**
   - Two editing tabs will appear. Close `ApplicationConfig.java` and implement the required functionalities in `GenericResource.java`.

     ![389206413-cef254e9-45db-4660-b1ea-01d3328e7ee1](https://github.com/user-attachments/assets/b01f0bf8-4e33-458e-a806-a91f1ef6b46f)


5. **Modify Method:**
   - Alter the `getHtml()` method as needed.

6. **Build and Deploy:**
   - Save your project, clean and build it. Deploy your project to the server.

     ![389206431-8722da37-9b0d-49b1-b5f5-d72f092a203b](https://github.com/user-attachments/assets/e68aa9c5-0087-4ad3-9ada-aecbcc11ee35)


7. **Test Your Web Service:**
   - Open a browser and type the URL `http://localhost:8080/project_name/webresources/generic?params=45&params=35` to test the web service functionality.

### Client-Side Implementation

1. **Create a New Java Web Project:**
   - Follow steps 1-5 from the SOAP-based Web Services section to set up a new Java Web Project.

2. **Create RESTful Java Client:**
   - Right-click on the project and select `New` -> `RESTful Java Client`.

   ![389206464-4d0066f0-975c-45e2-b66b-6b9f422905e2](https://github.com/user-attachments/assets/7598efb5-ae10-4b62-a540-b5579d40ae0a)


3. **Configure Client:**
   - In the new window, provide a name for your client, a package name, and select `From Project` under the `Select the REST resource:` tab. Click `Browse` and select your RESTful resource. Click `OK`, then `Finish`.

4. **Edit Client Code:**
   - Modify the `getHtml()` method as required.

     ![389206482-5d537bd1-4b0c-40cc-b6bb-20b9058c8ba2](https://github.com/user-attachments/assets/df8d41d1-6ab5-4ef6-b417-8303ba15cd25)


5. **Add JAR File:**
   - Right-click on the `Libraries` folder under your project and select `Add JAR/Folder`.
   - Navigate to where the `javax.ws.rs-api2.0.1.jar` file is located and add it.

     ![389206506-09f658dc-8046-4df6-9f29-b5d8c5bff358](https://github.com/user-attachments/assets/dabd704f-26f4-437c-adfc-a3e401bff039)


6. **Create JSP Page:**
   - Right-click on the `Web Pages` folder and select `JSP`.
   - Provide a name for the JSP page and click `Finish`.

     ![389206533-bd3e1ef3-00fb-457c-ae8a-54a8034eb1d1](https://github.com/user-attachments/assets/a56f64b9-4b20-4d7f-8f63-e99e41c0cb3a)


7. **Include Client Code in JSP:**
   - Edit the JSP page to include the necessary code for invoking the client Java code.

     ![389206552-f7b5695f-c4f3-47b6-82fb-5df7a8b4ab52](https://github.com/user-attachments/assets/87f320dc-5a65-4b07-b56b-47b32cfb1e04)


8. **Build and Run:**
   - Save the project, build it, and run the JSP file to see the output in a new browser window.

     ![389206587-9506ba81-47b7-49e3-88b6-b3d5a46f9eff](https://github.com/user-attachments/assets/05625e79-9567-47ab-9b23-917a6b8aeee8)

9. Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.

10. A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.

![389206669-5a734882-7282-4eea-b702-04ebf36b476c](https://github.com/user-attachments/assets/9540b75e-6dbf-4a16-9bca-aedad96fc85b)

11. Save the project and build it.

12. Run the JSP file and you should see the output in a new browser window.

![389206710-6669e150-ebd7-4826-bca8-8f8decff85a1](https://github.com/user-attachments/assets/c4622cd0-0072-4a68-a478-309c3f782333)

### Client-Side Remote Invocation (Optional)

1. **Adjust Client Configuration:**
   - Follow steps 1-5 from the Client-Side Implementation.
   - In the generated `NewJerseyClient.java` file, update `BASE_URI` from `private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources";` to `private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";`.

2. **Complete the Remaining Steps:**
   - Follow steps 6-12 from the Client-Side Implementation to finalize and test the remote client.

## Result

The implementation of RESTful web services using both server-side and client-side components was successfully created and executed.

