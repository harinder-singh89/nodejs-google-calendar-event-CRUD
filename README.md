## Project setup
```
npm install
```
## Run Project
```
node calendar.js
```
## How to create google calendar service

Step 1: Open google console and click on the dropdown for selecting a project. We will be creating a new project. Click on “NEW PROJECT” towards the top right. Give a suitable project name and click on create.

https://console.cloud.google.com/

Step 2: Google console dashboard will be displayed after creating a project. Make sure you are viewing the dashboard of your newly created project to add Google calendar functionality.

Step 3:  Click on APIs & Services tab present under the “More Products” section towards the left and then click on “Enable APIS and Services”.

Step 4:  The API library will be displayed. From here we can select which APIs we want to enable for our project. Since we are going to integrate Google calendar, type “Calendar” in the search box and select “Google Calendar API”.

Step 5:  All details of Google Calendar API will be displayed, including documentation and services of the API. Click on enable to add this API to your project.

Step 6:  Now we will be creating the service account for our application. Click on “CREATE CREDENTIALS” to create a service account.

Step 7: Select “Google Calendar API” as a type of API for the credential.

Step 8: Now you will be asked “What data will you be accessing?”, as we are creating a service account, click on “Application Data” and “Next”.

Step 9:  Next enter service account details such as account name and the service account ID will be generated simultaneously. Then click on “Create and Continue”.

Step 10:  We will select the “Owner” role for giving access to the service account to our application. After adding the role, click on continue.

Step 11:  This step is optional. It is up to you to give admin rights to a specific person or a group of people who can administer the service account. Click on Done.

Step 12:  The service account has been set up. Now the credentials for this service account have to be created. The key associated with this service account can be downloaded as a JSON file. We will refer to this as a “service key file” in later steps. Click on the email under Service Account.

Step 13:  Go to the KEYS tab and click on ADD KEY.

Step 14:  We will create a new key and select JSON as key type. Click on create.

Step 15: The private key is created and downloaded as a JSON file. Remember this file is highly sensitive and its credentials must not be public!

Step 16:  We still require the project number in order to configure the calendar. Click on the 3 dot menu option in the top right and click on “Project Settings”.

Step 17:  Copy the project number and store it in a safe place for future use.

Step 18: Now we will set up a Google calendar and retrieve its ID. The calendar will require credentials that we have got in the JSON file. Go to Google Calendar and create a new calendar by clicking ‘+’ beside “Other calendars”.

Step 19:  Enter name and description, then click on “Create calendar”.

Step 20:  Click on the 3 dot menu beside the newly created calendar and click on “Settings and sharing”.

Step 21:  Scroll down to the “Integrate calendar” section and copy the Calendar ID. Store this ID in a safe place for future use. Open the JSON service key file and copy “client email”. Go to the “Share with specific people” section and “Add people” by pasting the copied client email.
