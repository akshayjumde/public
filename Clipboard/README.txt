Step 1: Create a Firebase Account
-----------------------------------
Go to Firebase Console: Visit Firebase Console.
Sign In: Use your Google account to sign in.
Create a Project: Click "Add project" and name it. Click "Create project."

Step 2: Set Up Firestore Database
-----------------------------------
Open Firestore: Click "Firestore Database" in the left sidebar.
Create Database: Click "Create database" and select "Start in Test Mode." Click "Next."
Choose Location: Select a location and click "Done."

Step 3: Create a Collection
-----------------------------
Start Collection: Click "Start collection."
Name Collection: Enter "clipboard" as the name. Click "Next."
Add Document: Add a field:
Field Name: text
Type: string
Value: (leave blank or set default)
Click "Save."

Step 4: Get Firebase Configuration
-----------------------------------
Project Settings: Click the gear icon in "Project Overview."
Register App: Click the Web icon to register your app. Copy the configuration snippet.

Step 5: Set Up Security Rules
-------------------------------
Open Rules: Click on the "Rules" tab in Firestore.
Modify Rules: Update to secure settings, like below 

// json Copy code allow read, write: if request.auth != null; 

Publish: Click "Publish" to save rules.