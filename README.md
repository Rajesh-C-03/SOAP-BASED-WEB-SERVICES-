# SOAP-based Web Services

## Aim

To create SOAP-based web services using both server-side and client-side implementations.

## Procedure

### Server-Side Implementation

1. **Open NetBeans IDE:**
   - Launch NetBeans IDE on your machine.

2. **Create a New Project:**
   - Click `File` -> `New Project`.
   - Choose `Java Web` and then `Web Application`, and click `Next`.

3. **Configure Project:**
   - Provide a suitable name for your project and click `Next`.
   - Select `GlassFish Server` as the server and `Java EE 7 Web` as the Java EE version. Click `Finish`.

4. **Create a New Web Service:**
   - Right-click your project in the Projects tab and select `New` -> `Web Service`.

5. **Define Web Service:**
   - In the new window, give your web service a name and package name. Click `Finish`.

6. **Add Operation:**
   - Right-click on your web service under the “Web Services” folder in your project and select `Add Operation`.
   - In the window that appears, provide a name and return type for the operation. Click `Add` to define parameters (for demonstration, use two parameters). Click `OK`.

7. **Implement Operation:**
   - NetBeans will generate a skeleton for the operation. Replace `return 0.0` with `return (a+b)` to perform addition.
   - Save your project, right-click on it, and select `Clean and Build`. Then, right-click again and select `Deploy`.

8. **Test Web Service:**
   - Once deployed, right-click on the web service name and select `Test Web Service`.
   - A new browser window will appear where you can input values to test the web service.

### Client-Side Implementation

1. **Create a New Java Web Project:**
   - Follow steps 1-5 of the server-side section to create a new Java Web Project.

2. **Add Web Service Client:**
   - Right-click on your project and select `New` -> `Web Service Client`.
   - In the window that appears, select `Project` under “Specify the WSDL file of the Web Service” and click `Browse`.

3. **Select Web Service:**
   - Choose the appropriate web service and click `OK`.
   - Fill in the project file with the location of the WSDL file and provide a package name if desired. Click `Finish`.

4. **Verify and Build:**
   - The client will gather the available operations. Ensure “BUILD SUCCESSFUL” appears in the Output Window.

5. **Create JSP Page:**
   - Right-click on `Web Pages` under your project and select `JSP`.
   - Provide a name for your JSP page and click `Finish`.

6. **Invoke Web Service:**
   - Expand the folder `Web Service References` -> `Addition` -> `Addition` -> `AdditionPort`.
   - Drag and drop the `add` operation into the JSP page. NetBeans will auto-generate the code for invoking this operation.

7. **Run JSP Page:**
   - Provide values for the arguments and run the JSP file.
   - A new browser window will display the output of the web service invocation.

8. **Client-Side Remote Invocation (Optional):**
   - Follow steps 1-2 as in the client-side section.
   - Select `WSDL URL` and type the URL of the web service’s WSDL file (e.g., `http://ip:8080/Proj_name/Webservice_name?wsdl`).
   - Complete the remaining procedure as outlined.

## Result

The SOAP-based web services were successfully created and executed, demonstrating both server-side and client-side implementations.

