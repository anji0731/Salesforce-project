# Current Project Status
Phase 1: Problem Understanding & Requirements: Complete

Phase 2: Org Setup & Configuration: Complete

Phase 3: Data Modeling & Relationships: Complete

Phase 4: Process Automation (Admin): Not Started

Phase 5: Apex Programming (Developer): Not Started

Phase 6: User Interface Development: Not Started

Phase 7: Integration & External Access: Not Started

Phase 8: Data Management & Deployment: Not Started

Phase 9: Reporting, Dashboards & Security Review: Not Started

Phase 10: Final Presentation & Delivery: Not Started


## Salesforce Project - Leave Tracker App

This repository contains my Salesforce Leave Tracker capstone projec.

## Project Documentation
You can view the full documentation here:  
[Click here to open Google Doc](https://docs.google.com/document/d/1eVC8uJEWHhLEBpZxbIhLQaiBj1SMUSgegaTd3MN68sk/edit?tab=t.0#heading=h.y2995cnn5dwm)

This is a custom Leave Management application built on the Salesforce Platform using Lightning Web Components (LWC). This project was created to address the inefficiencies of manual leave tracking and provides a centralized, automated system for employees and managers.


## 1.Problem Statement

Currently, the company handles employee leave requests through emails and spreadsheets. This causes mistakes like double bookings, lost requests, and no real-time tracking. A centralized automated system is needed to make leave management easier and more accurate.

## 2.Technology Stack

**Platform**: Salesforce

**Frontend**: Lightning Web Components (LWC), HTML, CSS

**Backend**: Apex (for server-side logic and queries)

**Database**: Salesforce Platform (Custom Objects & Fields)

**Tools**: Salesforce CLI, Visual Studio Code, Git, GitHub

## 3.Key Features

**Leave Request Submission**: A user-friendly LWC form for employees to submit new leave requests with an intuitive date picker.

**Automated Validation**: Custom validation rules to prevent submitting requests with incorrect dates.

**Real-time Visibility**: An LWC that displays an employee's leave history in a sortable data table, with a real-time status update.

**Manager Approvals**: A custom approval process that automatically routes requests to the appropriate manager.

**Robust Backend Logic**: Apex triggers to prevent any overlapping leave requests for the same employee, ensuring data integrity.

**Data Modeling**: Implementation of the `Leave_Request__c` custom object and its relationships to the `User` object.

## 4. Installation and Setup
1.  **Clone the Repository:**
    `git clone https://github.com/anji0731/Salesforce-project.git`

2.  **Authorize Your Salesforce Org:**
    `sfdx force:auth:web:login`

3.  **Deploy Source to Your Org:**
    `sfdx force:source:deploy --sourcepath force-app`

4.  **Assign Permission Sets:** Assign the appropriate permission sets to users to access the `Leave_Request__c` object and the Lightning components.

5.  **Add to a Lightning Page:** Use the Lightning App Builder to drag and drop the `leaveTracker` component onto an App Page.