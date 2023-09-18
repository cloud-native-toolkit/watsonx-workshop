# Lab-guide-Techzone Integrating Watson Discovery, Watson Assistant and WatsonX

**1. Creating Watson Discovery instance**

Perform this step to create a Watson Discovery instance.

First, go to https://cloud.ibm.com/resources where you need to click the "Create resource" button

![image](https://media.github.ibm.com/user/269035/files/4f3723ae-3058-4235-b4d2-ac1d76296769)


Then search in the resource directory for Watson Discovery (1.) and then select it (2.)


![image](https://media.github.ibm.com/user/269035/files/fa9713fe-3c2a-48b5-aed9-a1fe786e3d6b)


Select the instance location that suits you (Dallas by default) (1.). Then pricing the plan that matches your expectations. (2.) Accept the license terms. (3.) And finally, click the "Create" button. (4.)

![image](https://media.github.ibm.com/user/269035/files/86b9e6a6-296d-4e73-bcd9-29b81a5dd496)

**2. Accessing Watson Discovery instance**

Once you have a Watson Discovery instance, it will be available at https://cloud.ibm.com/resources under the AI / Machine Learning category. Click on it to proceed further.

![image](https://media.github.ibm.com/user/269035/files/7244fc79-9927-4d0c-9cb4-b13f75fd3642)


Once in the instance, click on the "Launch Watson Discovery" button to start working with it. (1.)

![image](https://media.github.ibm.com/user/269035/files/e0aa78c9-b7e8-49aa-9745-c6b89442593b)


NOTE: On the current sub-page, you may notice a Credentials section where you can find the API key and URL that you will need in the next steps for configuration. (2.)

![image](https://media.github.ibm.com/user/269035/files/54ff0bc4-6d0c-4c8e-ba7d-45c48f508877)

**3. Creating new project**

Now, in order to start working on your documents, you need to create a new project by clicking on the "New project" button

![image](https://media.github.ibm.com/user/269035/files/40dea999-5813-445c-900c-67f5e6a30a6f)

Give a name to your project (1.), select Project type "Document Retrieval" (2.) and proceed by clicking the "Next" button. (3.)

![image](https://media.github.ibm.com/user/269035/files/082a847e-cf7a-4499-8257-988a938f7356)


Choose where you want to upload your data from - in this case I'm using a local file (2 zip files inside datasets folder), so I choose "Upload data" (1.), and then click "Next."(2.).  Please create 2 different collections for both datasets as "Products" and "ProductReviews" collections.

IMG

<img width="452" alt="image" src="https://media.github.ibm.com/user/269035/files/ab3ef7b1-9675-4450-88d9-f678a97bdd58">

create the name of the collection 

<img width="452" alt="image" src="https://media.github.ibm.com/user/269035/files/a35270e1-d6b0-4de2-984d-295522d61a6a">

I select the appropriate file (1.) and then click "Finish".

We are automatically transferred to the created project. It is also available within the list of projects available by clicking on "My Projects" in the menu at the top.

**4. Working in the project**

While in the corresponding project. In the menu on the left, we go to the "Manage Collections" section.

Then we enter our newly created collection.

Note that Watson Discovery takes a while to process the documents loaded into it, so "Documents available" may be 0.

After entering the collections, we see how many documents are still processing and how many are available. When all the documents have processed in our case we created 2 collections Review and Products-retails as shown in the below image.

<img width="452" alt="image" src="https://media.github.ibm.com/user/269035/files/a7fa366d-184b-476b-996f-71a5a9fb30a2">

![image](https://media.github.ibm.com/user/269035/files/fdd84695-3b86-42a6-b47c-e17c8c15340e)


**Using Postman to Query Watson Discovery Collection**


Objective: In this lab, you will learn how to use Postman to query a Watson Discovery Collection, import environment variables, and execute a POST request to retrieve relevant passages.
Prerequisites:
•	Access to Postman (If not installed, you can download it from https://www.postman.com/ or use a web version)
•	A Google Account

Step 1: Access Postman
1.	Open your web browser and go to Postman's website.
2.	Click on sign in"

<img width="1419" alt="image" src="https://github.com/cloud-native-toolkit/watsonx-workshop/assets/73220577/9ac4e0d8-c7fe-4755-8bf8-73d46c947ee3">
   
Step 2: Login to Postman through Google Account
1.	Open Postman.
2.	Click on "Sign In" in the upper right corner.
3.	Select "Continue with Google."
4.	Sign in with your Google Account.
5.	Create workspace
6.	from dataset file download RetailCollection.postman_collection.json(Discovery queries) and RetailDemo.postman_environment.json (envirnoment variables)

Step 3: Import Environment Variables
1.	In Postman, click on "Environments" in the top right corner.
2.	Click on "Import."
3.	Choose the environment variables file you want to import (usually in JSON format).
Step 4: Import Queries
1.	In Postman, click on "Import" in the top left corner.
2.	Choose "File" and select the JSON file containing your queries.
   
Step 5: Run the Query
1.	In Postman, select the RetailCollection.postman_collection.json or request where you imported the queries.
2.	On the right side, under "Params" or "Body," ensure that you've selected the right environment variable for your query.
3.	Click on "Send" to execute the POST request.
4.	Review the response to see the relevant passages fetched from the Watson Discovery Collection.

Note: Post query looks like these {{wd_service_url}}/v2/projects/{{wd_project_id}}/query?version=2020-08-30 were **wd_service_url** and **wd_project_id}** are fetched from Envirnoment variables.

<img width="1376" alt="image" src="https://github.com/cloud-native-toolkit/watsonx-workshop/assets/73220577/aeb32dc1-7e07-4e32-877f-e90015f97bbd">
   
Congratulations! You have successfully used Postman to query a Watson Discovery Collection, imported environment variables, and executed a POST request to retrieve relevant passages.




