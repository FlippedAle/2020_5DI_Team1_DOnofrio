# <a id="top"></a> Software Requirements Specifications

Version 1.0,  
prepared by TheFlippedCompany

## Table of Content

1. [Introduction](#introduction)  
   1.1 Overview  
   1.2 Goals  
   1.3 Definitions
2. [General Design Constraints](#gdc)  
   2.1 OnGo Application Environment  
   2.2 User Characteristics  
   2.3 Mandated Constrains  
3. [Nonfunctional Requirements](#nfr)  
   3.1 Operational Requirements  
   3.2 Performance Requirements  
   3.3 Security Requirements  
   3.4 Documentation and Training  
   3.5 [External Interface](#ei)  
      &nbsp;&nbsp;&nbsp;3.5.1 User Interface  
      &nbsp;&nbsp;&nbsp;3.5.2 Software Interface
4. [Functional Requirements](#fr)  
   4.1 Required Features  
      &nbsp;&nbsp;&nbsp;4.1.1 Use Case 1 - Create a Folder  
      &nbsp;&nbsp;&nbsp;4.1.2 Use Case 2 - Tranfer a file to the origin  
      &nbsp;&nbsp;&nbsp;4.1.3 Use Case 3 - Require a file from the origin  
   4.2 Optional Features  
      &nbsp;&nbsp;&nbsp;4.2.1 Use Case 1 - Send a command from a CLI  
      &nbsp;&nbsp;&nbsp;4.2.2 Use Case 2 - Create a file with content

## 1. <a id="introduction"></a> Introduction

### 1.1 _Overview_

The **OnGo** is an application that provides you access to all the files stored on your personal computer from _any device_ you want.

This document provides informations on the requirements for the **OnGo** application.  
Project goals, scope and definitions are given in the _introduction_.  
_Design constraints_ and _application environment_ are described in the following section.  
_Nonfunctional requirements_ are outlined for later verification.  
_Functional requirements_ are given to show the system features and expected user interaction.  
The _Software Project Management Plan_ will give specifics on project budget and schedule.

### 1.2 _Goals and Objectives_

The **main objective** of this project is to allow users to have an easy and quick access to any file stored on other devices. The OnGo application is expected to: 

* function in an **simple and intuitive** manner
* provide an **easy access** to the user's files without   uploading them first, as cloud services require to.
* work on **any** operative system and device

### 1.3 _Definitions_

> **Origin** - It's the computer on which files are _actually_ stored, your "_home pc_" if you want to.

> **User** - It's the person that's trying to get to the _origin_ via OnGo

## 2. <a id="gdc"></a> General Design Constrains

### 2.1 _Application Environment_

The OnGo product includes:

* A **desktop application** of our design that has to be installed on the _origin_ system
* A **web application** of our design that is used by the _user_ to interact with his own registered _origin_ system

Both applications interact with our [Web Api][OnGoApi] that will handle the communications between the **user** and the corresponding **origin**. 

### 2.2 _User Characteristics_

Users will need to have a valid [account][FlippedWebsiteLogin] in order to download the **OnGo origin program** and they will also need to use their accounts to log into the **user web application** in order to use it. There is _no limitation_ on the device that the user can use.

### 2.3 _Mandated Constrains_

The whole system has to work via HTTP connection (https). This is mandatory because the _origin_ machine will probably be inside a private network and it might not be allowed to host a server accessible from the public internet due to several security issues or privacy policies. 

## 3. <a id="nfr"></a> Nonfunctional Requirements

### 3.1 _Operational Requirements_

The **user web application** has to provide an easy to use interface and should be simple enough to let every user connect to it's own origin without any serious problems.

The **origin main application** has to generate and give the code to the user in the most clear way possible. The user will still need to remember that code by himself.

### 3.2 _Performance Requirements_

When a file is _downloaded_ / _uploaded_, the system has to deliver the whole document without losing any part regardeless of the file dimension.

### 3.3 _Security Requirements_

The first versions of the OnGo application will only require:

* User **login** and **registration** (to download the origin application and to use the user web app)

### 3.4 _Documentation and Training_

The OnGo application _itself_ will not include any documentation or training for the final user but video tutorials will be available on the [team website][FlippedWebsite] and on the official [YouTube channel][FlippedYoutubeChannel].

### 3.5 <a id="ei"></a> _External Interface_

#### 3.5.1 _User Interface_

The interface will be _eye-catching_ in order to let the user interact with a _familiar environment_.

The interface will be easy to use on any device since it will resemble a _Windows-like operating system UI_.

#### 3.5.2 _Software Interface_

The [OnGo Api][OnGoApi] works as an interface between the **origin** application and the **user** application. It handles and direct all the communications between the _users_ and their corresponding _origin_ system.

## 4. <a id="fr"></a> Functional Requirements

### 4.1 _Required Features_

#### 4.1.1 _Use Case 1_

**Description: Create a new folder and navigate inside it**  
Actors: OnGo _User_  

Basic path _origin_:
1. The user opens the _OnGo Desktop Application_
2. The user copies the generated code
3. _The user can now decide when to start working on his other devices_

Basic path _user_:  
1. The user goes to [our website][FlippedWebsite]
2. The user clicks on the _OnGo Application Icon_
3. The user _logs into_ his account
4. The user prompts the _previously given_ code
5. The system provides an _accurate view_ of the user's origin system
6. The user navigates to the desired folders by _double-clicking_ on them
7. To create a new folder, the user _right-clicks_ on the page and clicks on "_New folder_"
8. The user decides a proper name and then clicks _create_
9. A new folder has just been created on the origin system

#### 4.1.2 _Use Case 2_

**Description: Transfer a file from the User to the Origin**  
Actors: OnGo _User_  

Basic path _origin_:
1. The user opens the _OnGo Desktop Application_
2. The user copies the generated code
3. _The user can now decide when to start working on his other devices_

Basic path _user_:  
1. The user goes to [our website][FlippedWebsite]
2. The user clicks on the _OnGo Application Icon_
3. The user _logs into_ his account
4. The user prompts the _previously given_ code
5. The system provides an _accurate view_ of the user's origin system
6. The user navigates to the desired folders by _double-clicking_ on them
7. To transfer a document, the user _drags and drops_ the desired file from the local system to the web application
8. A new file has just been transfered to the origin system

#### 4.1.2 _Use Case 3_

**Description: Require a file located in the Origin as a User**  
Actors: OnGo _User_  

Basic path _origin_:
1. The user opens the _OnGo Desktop Application_
2. The user copies the generated code
3. _The user can now decide when to start working on his other devices_

Basic path _user_:  
1. The user goes to [our website][FlippedWebsite]
2. The user clicks on the _OnGo Application Icon_
3. The user _logs into_ his account
4. The user prompts the _previously given_ code
5. The system provides an _accurate view_ of the user's origin system
6. The user navigates to the desired folders by _double-clicking_ on them
7. The user, to require a file, _right-clicks_ on the desired document and clicks on "_Download_"
8. After a few seconds, the required file is downloaded on the user's system 

### 4.2 _Optional Features_

#### 4.2.1 _Use Case 1_

**Description: Send a full proper command through a DOS emulator. Computer shutdown from CLI**  
Actors: OnGo _User_  

Basic path _origin_:
1. The user opens the _OnGo Desktop Application_
2. The user copies the generated code
3. _The user can now decide when to start working on his other devices_

Basic path _user_:  
1. The user goes to [our website][FlippedWebsite]
2. The user clicks on the _OnGo Application Icon_
3. The user _logs into_ his account
4. The user prompts the _previously given_ code
5. The system provides an _accurate view_ of the user's origin system
6. The user clicks on the _CMD_ icon on the top-left corner
7. A CLI will appear in the view and the user will be able to send proper commands
8. To shut the system down in 60 seconds, the user types _sudo shutdown -s -t 60_
9. The system will be shut down and the connection will be closed

#### 4.2.2 _Use Case 2_

**Description: Add a new file with content in it**  
Actors: OnGo _User_  

Basic path _origin_:
1. The user opens the _OnGo Desktop Application_
2. The user copies the generated code
3. _The user can now decide when to start working on his other devices_

Basic path _user_:  
1. The user goes to [our website][FlippedWebsite]
2. The user clicks on the _OnGo Application Icon_
3. The user _logs into_ his account
4. The user prompts the _previously given_ code
5. The system provides an _accurate view_ of the user's origin system
6. The user navigates to the desired folders by _double-clicking_ on them
7. To create a new file, the user clicks on the _Notepad_ icon on the top-left corner
8. When the web editor loads up, the user will be able to type and save the document in the desired format by clicking the "_save_" button
9. The user will then type the desired name and extension in the modal
10. A new file with content _has been added_ to the origin system in the desired path

#### [Top page](#top)
#### [Index](index.md)

[FlippedWebsite]: https://www.theflippedteam.altervista.org
[OnGoApi]: https://us-central1-web-ftp-ongo.cloudfunctions.net/api
[FlippedWebsiteLogin]: https://www.theflippedteam.altervista.org
[FlippedYoutubeChannel]: https://www.youtube.com
