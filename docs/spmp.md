# <a id="top"></a> Software Project Management Plan 

Version 1.0,  
prepared by TheFlippedCompany

## Table of Content

1. [Overview](#overview)  
   1.1 Definitions  
   1.2 Purpose and Scope  
   1.3 Goals and Objectives  
   1.4 Projects Deliverables  
   1.5 Assumptions and Constraints  
   1.6 Schedule and Budget Summary  
      &nbsp;&nbsp;&nbsp;1.6.1 Schedule  
      &nbsp;&nbsp;&nbsp;1.6.2 Budget  
   1.7 Success Criteria
2. [Startup Plan](#startupPlan)  
   2.1 Team Organization  
   2.2 Project Communication  
   2.3 Technical Process  
   2.4 Tools  
3. [Work Plan](#workPlan)  
   3.1 Activities and Tasks   
   3.2 Release Plan  
4. [Control Plan](#controlPlan)  
   4.1 Monitoring and Control   
   4.2 Project Measurements  
5. [Supporting Process Plans](#processPlans)  
   5.1 Risk Management Plan  
   5.2 Test Plan  
   5.3 Product Acceptance Plan

## 1. <a id="overview"></a> Overview

### 1.1 _Definitions_

**OnGo** – the product that has being described here; the application specified in this document 
**Origin** – it is the computer on which files are actually stored
**User** – it is the actual device on which the OnGo user is working with

### 1.2 _Purpose and Scope_

The OnGo application provides access to files located on a remote computer, without the necessity of uploading them on any cloud service. There is no such a problem as not finding the needed file because with OnGo users work directly with all files on the origin. 

The purpose of this project is to easily work with files on devices nowhere near the user.

### 1.3 _Goals and Objectives_

The main objective of OnGo is to allow users to have an easy and quick access to any file stored on their devices. The OnGo application is expected to:  
* function in a simple and intuitive manner 
* provide an easy access to the user’s files without uploading them first, as cloud services required to 
* work on any operative system and device 

### 1.4 _Project Deliverables_

There are no extra outputs of the project delivered to the costumers, such as a source code, user’s guide or any manual.  Video tutorials will be avaible on the team website and on the official YT Channel.

### 1.5 _Assumptions and Constraints_

Assumptions:
* The OnGo system takes advantage of the HTTP technology
* The OnGo app will work on any device

Constrains:
* The documentation must be ready by 01/05/2020
* Users will need to remember the code to pair the origin and the user by themselves

### 1.6 _Schedule and Budget Summary_

#### 1.6.1 _Schedule_

* 27/11/19 – Brainstorming ideas on OnGo application (general purpose and name decisions)
* 28/11/19 – Design architecture and sketching down the project 
* 04/12/19 – Project Plan and group subdivision 
* 05/12/19 – Project Presentation 
* 11/12/19 – Application and documentation developing 
* 12/12/19 – Application and documentation developing 
* 19/12/19 – Application and documentation developing

*extra-work dates are not included*

#### 1.6.2 _Budget_

There’s no total project cost, for now it will be a no-profit project

### 1.7 _Success Criteria_

A working prototype, which is easy to use, that allows users to access to any of their file located on a remote computer from any device.

## 2. <a id="startupPlan"></a> Startup Plan

### 2.1 _Team Organization_

* Role: Project Manager  
Actor(s): D’Onfrio Alessandro  
Responsibility: break out tasks, assign them to teammates, call team meetings  

* Role: Communication Coordinator  
Actor(s): Brighenti Christine  
Responsibility: Coordinate communications within group, coordinate communications outside group  

* Role: Programmer  
Actor(s): Ricca Emanuele, D’Onofrio Alessandro, Ferrari Matteo  
Responsibility: Program to requirement and architect specifications  

* Role: Developer  
Actor(s): Ricca Emanuele, D’Onofrio Alessandro  
Responsibility: Develop software based on requirement and architect specifications  

* Role: Requirement Engineer  
Actor(s): Brighenti Christine, D’Onofrio Alessandro  
Responsibility: Outline and document project requirements

### 2.2 _Project Communication_

Event: Team Meeting  
Information: Task status, completed since last meeting & planned for next  
Audience: All team members  
Format: Informal meetings and WhatsApp messages status updates & problems as they occur  
Frequency: Everyday  

Event: Project Status Report  
Information: Review finished items and programming issues  
Audience: All team members  
Format: WhatsApp messages  
Frequency: As needed  

### 2.3 _Technical Process_

An iterative and incremental development process is planned.  Feedback will be used from each iteration to improve the next.  The first iteration will focus on basic functionality of the application.  Subsequent iterations will build upon that and incorporate more features as time allows.

### 2.4 _Tools_

* Programming & Markup Languages - Python, NodeJS, JavaScript, HTML, CSS, Firebase DB, Firebase Functions, Firebase Hosting, Google Storage
* Operating System - Any
* Version Control - GitHub Inc.

## 3. <a id="workPlan"></a> Work Plan

### 3.1 _Activities and Tasks_

Detailed resource estimates will be available on the website.

### 3.2 _Release Plan_

**Iteration #1**

Date: 27/11/2019 – 20/12/2019  
Summary: OnGo basic and fundamental architecture

Feature: Server application architecture  
Estimated effort: 50  
Actual effort: 40  
Features: Tester Application for requests and operations  
Estimated effort: 50  
Actual effort: 60

**Iteration #2**

Date: 18/12/2019 – 20/12/2019  
Summary: integration with helpful platforms   

Feature: Firebase Integration  
Estimated effort: 50  
Actual effort: 70  

Date: 22/12/2019 – 27/12/2019  
Feature: Bucket configuration Google Storage  
Estimated effort: 40  
Actual effort: 50  

**Iteration #3**

Date: 23/12/2019 – 27/12/2019  
Summary: Taking care of file transfer 

Feature: User interface  
Estimated effort: 70  
Actual effort: 70  

**Iteration #4**

Date: 27/11/2019 - …  
Summary: Developing user interface  

Feature: User interface  
Estimated effort: 70  
Actual effort: 70

## 4. <a id="controlPlan"></a> Control Plan

### 4.1 _Monitoring and Control_

Daily: Team meeting. Project participants report status, progress and potential problems

* 27/11/2019 – discussion on the realization of the whole project  
11/12/2019 – critical tests on request to the server  
23/12/2019 – critical tests on file exchange 

Milestones are included to reference down below:

* Date: 20/12/2019  
Milestone: Iteration #1

* Date: 20/12/2019  
Milestone: Iteration #2

* Date: 27/12/209  
Milestone: Iteration #3

### 4.2 _Project Measurements_

The following procedure is to be used when making changes to all baselined work products, as a team we decided to follow an already existing procedure:

1. All project work products will be stored in a centralized repository.
2. All project work products (documents, source code, test cases, program data, test data, etc) will be stored in a repository (subject to formal change control procedures.) 
3. Items that are subject to change control will be considered baselined after a group review at the end of the initial document creation.  
4. The change control procedure once a product is baselined is:  
    &nbsp;&nbsp;&nbsp;4.1 anyone wanting to make a change to a baselined item sends a message to the rest of the team describing the change, reason for the change, expected schedule impact, and time line for integrating the change.  

    &nbsp;&nbsp;&nbsp;4.2 if no one responds to the group within 2 days with a reason for why the change request shouldn't be permitted, it will be considered accepted and the person proposing the change may proceed with the change. 

    &nbsp;&nbsp;&nbsp;4.3 if anyone does object to the change, the reason for objecting will be discussed at a meeting where everyone is invited to attend and voice their opinion. At the end of the meeting a democratic vote will be held to decide whether or not the change should be allowed.  

    &nbsp;&nbsp;&nbsp;4.4 if a change takes place, the initiator must collaborate with the project manager to update the schedule.

## 5. <a id="processPlans"></a> Supporting Process Plans

### 5.1 _Risk Management Plan_

* Rank: 1  
Risk: Schedule  
Probability of loss: Likely  
Size of loss: Major  
Risk exposure: High  
Response: Stick to the schedule

* Rank: 2  
Risk: Tester Application  
Probability of loss: Likely   
Size of loss: High  
Risk exposure: High  
Response: Avoid – avoid simple errors and follow the outline

* Rank: 3  
Risk: Deploy error  
Probability of loss: High  
Size of loss: High  
Risk exposure: Moderate  
Response: Avoid – avoid any error and follow the right procedures 

### 5.2 _Test Plan_

The test plan defines the items that will be tested, methods for testing, and a schedule detailing the tasks, owners, and time line.

The test plan will be available in a separate document on the website.

### 5.3 _Product Acceptance Plan_

At the conclusion of each iteration, the prototype created will tested to ensure it meets the requirements of that iteration. For the final iteration, product acceptance testing will ensure that the prototype functions as expected.

#### [Top page](#top)
#### [Index](index.md)

[FlippedWebsite]: https://www.theflippedteam.altervista.org
[OnGoApi]: https://us-central1-web-ftp-ongo.cloudfunctions.net/api
[FlippedWebsiteLogin]: https://www.theflippedteam.altervista.org
[FlippedYoutubeChannel]: https://www.youtube.com