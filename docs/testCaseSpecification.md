
# Sailor - Pioneers of the digital entrepreneurship
## Test Case Specification        

### **Revision History**

| Version | Modifier | Date       | Description of Change |
|:-------:|:--------:|:----------:|:----------------------|
| 0.1 | A. D'Onofrio | 14/04/2020 | Initial roigh draft.  |

## 1. Introduction

This document provides the test cases to be carried out for the Sailor platform.  
Each test is represented by a test case together with the input and expected outputs.

## 2. Test Cases

### 2.1 - Login to the Sailor platform

| Test ID | Title | Feature | Objective | Test Data | Expected Results |
|:-------:|:-----:|:--------|:----------|:----------|:-----------------|
|2.1|Succesful Login|Login to the Sailor platform|Confirm that after a correct login the user is prompted to his/her profile|Email: theflippedguys@gmail.com, Password: Prova123|The system redirects you to the user profile|

### 2.2 - Login to the Sailor platform

| Test ID | Title | Feature | Objective | Test Data | Expected Results |
|:-------:|:-----:|:--------|:----------|:----------|:-----------------|
|2.2|Failed Login 1|Login to the Sailor platform|Confirm that the system does not allow anyone to log in with the wrong credentials|Email: theflippedguys@gmail.com, Password: Errore|The system shows a message containing the correct error code, informations and possible fixes|

### 2.3 - Login to the Sailor platform

| Test ID | Title | Feature | Objective | Test Data | Expected Results |
|:-------:|:-----:|:--------|:----------|:----------|:-----------------|
|2.3|Failed Login 2|Login to the Sailor platform|Confirm the system ability to recognize if an account does not exist by denying the access to anyone who tries to log in without a registered email|Email: theflippedteam@gmail.com, Password: Prova123|The system shows a message containing the error correct code, informations and possible fixes|

### 2.4 - Purchases

| Test ID | Title | Feature | Objective | Test Data | Expected Results |
|:-------:|:-----:|:--------|:----------|:----------|:-----------------|
|2.4|Succesful Purchase|Purchases|Confirm that the system will correctly register an order once being forwarded by the client|An example order with the previously used account (theflippedguys@gmail.com)|The system will correctly register the order in the database and it will be visible by the staff in the pending orders dashboard and by the user in the appropriate section|

### 2.5 - Purchases

| Test ID | Title | Feature | Objective | Test Data | Expected Results |
|:-------:|:-----:|:--------|:----------|:----------|:-----------------|
|2.5|Failed Purchase|Purchases|Confirm that the system can succesfully detect a non-valid order request|An example order with the previously used account but deselecting every item from the list before forwarding it|The system shows a message containing the error correct code, informations and possible fixes. It also will not proceed with the actual payment procedure nor register the order in the database|


### 2.6 - Purchases

| Test ID | Title | Feature | Objective | Test Data | Expected Results |
|:-------:|:-----:|:--------|:----------|:----------|:-----------------|
|2.6|Succesful Order Redeem|Purchases|Confirm that the system will download the finalized order onto the user machine and record the actions in the database|The previously used example order forwarded by the example account|The system will download the complete package onto the user's machine and also record the succesful checkout|

### 2.7 - Puchases 

| Test ID | Title | Feature | Objective | Test Data | Expected Results |
|:-------:|:-----:|:--------|:----------|:----------|:-----------------|
|2.7|Failed Order Redeem|Purchases|Confirm that the system will signal an error and communicate it to both client and staff|This exact error cannot be caused voluntarily, so the user will need to communicate it via a button that triggers the issue procedure|The system records that a user has an issue downloading the order by setting a flag in the status field in the database and sending a mail notification to the staff that will work on a fix as soon as possible|
