# Salesforce Project - Leave Tracker App

This repository contains my Salesforce Leave Tracker App project.

## Project Documentation
You can view the full documentation here:  
[Click here to open Google Doc](https://docs.google.com/document/d/1eVC8uJEWHhLEBpZxbIhLQaiBj1SMUSgegaTd3MN68sk/edit?tab=t.0#heading=h.y2995cnn5dwm)

This is a custom Leave Management application built on the Salesforce Platform using Lightning Web Components (LWC). This project was created to address the inefficiencies of manual leave tracking and provides a centralized, automated system for employees and managers.

1. **Problem Statement**
Start with a strong, clear problem statement. This shows that you understand the business context and are not just building a technical artifact.

Problem Statement:
The company is currently managing all employee leave requests manually through email and spreadsheets. This system is inefficient and prone to errors, leading to double-booked time off, lost requests, and a lack of real-time visibility. This project aims to create a centralized, automated system to streamline the entire leave management process and ensure accuracy.

2. **Technology Stack**
List the technologies you used. This is crucial for your mentor and for future employers to see your technical skills at a glance.

Technology Stack:

Platform: Salesforce

Frontend: Lightning Web Components (LWC), HTML, CSS

Backend: Apex (for server-side logic and queries)

Database: Salesforce Platform (Custom Objects & Fields)

Tools: Salesforce CLI, Visual Studio Code, Git, GitHub

3. **Key Features**
Expand on the features we've already discussed. Be specific about what each feature does.

Key Features:

Leave Request Submission: A user-friendly LWC form for employees to submit new leave requests with an intuitive date picker.

Automated Validation: Custom validation rules to prevent submitting requests with incorrect dates.

Real-time Visibility: An LWC that displays an employee's leave history in a sortable data table, with a real-time status update.

Manager Approvals: A custom approval process that automatically routes requests to the appropriate manager.

Robust Backend Logic: Apex triggers to prevent any overlapping leave requests for the same employee, ensuring data integrity.

Data Modeling: Implementation of the Leave_Request__c custom object and its relationships to the User object.

4. **Installation and Setup**
This is a critical section for any collaborative project. It shows that your work is easy to set up and use.

Installation and Setup:

Clone the Repository:
git clone https://github.com/anji0731/Salesforce-project.git

Authorize Your Salesforce Org:
sfdx force:auth:web:login

Deploy Source to Your Org:
sfdx force:source:deploy --sourcepath force-app

Assign Permission Sets: Assign the appropriate permission sets to users to access the Leave_Request__c object and the Lightning components.

Add to a Lightning Page: Use the Lightning App Builder to drag and drop the leaveTracker component onto an App Page.