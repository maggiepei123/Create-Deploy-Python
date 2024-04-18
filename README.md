# Create-Deploy-Python
In this project, you will learn to deploy your own Python program on the Azure DevOps pipeline.
Here is some very detailed manual.

## Create Local Project
1. Choose the Azure icon in the Activity bar, then in the Azure: Functions area, select the “Create new project…” icon.

2. Choose a directory location for your project workspace and choose Select.

3. Provide the following information at the prompts:

Select a language for your function project: Choose Python.
Select a Python alias to create a virtual environment: Choose the location of — your Python interpreter.
If the location isn’t shown, type in the full path to your Python binary.
Select a template for your project’s first function: Choose HTTP trigger.
Provide a function name: Type HttpExample.
Authorization level: Choose Anonymous, which enables anyone to call your function endpoint. Select how you would like to open your project: Choose Add to workspace.

4. Using this information, Visual Studio Code generates an Azure Functions project with an HTTP trigger. You can view the local project files in the Explorer.
![image](https://github.com/maggiepei123/Create-Deploy-Python/assets/165247682/3b606bb2-c804-43a0-ad55-538d6ad2d1eb)

## Run Local Project
1. Click the RUN AND DEBUG button on the left of the function bar
![image](https://github.com/maggiepei123/Create-Deploy-Python/assets/165247682/1d77c457-2f45-4803-91de-0e01e1ab1148)
Choose use local emulater
![image](https://github.com/maggiepei123/Create-Deploy-Python/assets/165247682/fa2def5b-1049-4876-af42-e2b052107a44)

2. With Core Tools running, go to the Azure: Functions area. Under Functions, expand Local Project > Functions. Right-click (Windows) the HttpExampleProject function and choose Execute Function Now.
![image](https://github.com/maggiepei123/Create-Deploy-Python/assets/165247682/45744b1d-cc6b-4ba5-95f9-c319c68db79c)

3. In the “Enter request body,” you see the request message body value of { “name”: “Azure” }. Press Enter to send this request message to your function.

4. When the function executes locally and returns a response, a notification is raised in Visual Studio Code. Information about the function execution is shown in the Terminal panel.

5. Press Ctrl + C to stop Core Tools and disconnect the debugger.

##Create Azure Function APP 

1. Log in Azure portal and click on Create Resource or you can search for Function app from the search bar to create and give required fields such as app name, storage account, and resource group, runtime stack(Python).
![image](https://github.com/maggiepei123/Create-Deploy-Python/assets/165247682/1a6d5f7a-1914-46e1-80a5-ba2e16a79af2)

##Build pipeline on Azure DevOps

1. Log in your account in https://dev.azure.com/ and create a project.
2. Create a Repo and Put your code in Azure Repos. Repository should be imported from github. Therefore, you need to update your local repository on github first. Use the Github Desktop for importing can be very convenient.
REMEMBER to set your repository's visibility on github to public 
![image](https://github.com/maggiepei123/Create-Deploy-Python/assets/165247682/b625b8fe-1171-495c-a2a6-8a87281c3db9)
![image](https://github.com/maggiepei123/Create-Deploy-Python/assets/165247682/c41fbf34-68d6-4c79-af6c-90c71b706803)
3. Create a build pipeline
![image](https://github.com/maggiepei123/Create-Deploy-Python/assets/165247682/490a32ce-ec5a-4808-82bc-a489c8e4921e)
Let’s create a pipeline by selecting a source and repository branch and by selecting a classic editor.
![image](https://github.com/maggiepei123/Create-Deploy-Python/assets/165247682/8b7e9678-f841-4f81-a46a-2e1bc7f2aadd)

4. Release the pipeline
![image](https://github.com/maggiepei123/Create-Deploy-Python/assets/165247682/12381fcb-0c6e-4d1c-939c-68b7a2d0c319)


##Demo
![image](https://github.com/maggiepei123/Create-Deploy-Python/assets/165247682/a7c4bf66-7dc9-4480-a444-2517f12abf7b)





