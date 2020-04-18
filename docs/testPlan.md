# Sailor - Pioneers of the digital entrepreneurship
## Test Plan       

### **Revision History**

| Version | Modifier | Date       | Description of Change |
|:-------:|:--------:|:----------:|:----------------------|
| 0.1 | E. Ricca     | 14/04/2020 | Initial rough draft.  |

## 1. Introduction

This document defines the test plan for the project "Sailor".  
The platform will provide people with low skills in the tech fields the possibility to start their own online business by purchasing different assets that may not be possible for them to make.  
The testing routine will test the proper operation of the buying system and the login system.  
The results of the test will be used to fix possible bugs and increase the overall quality level of the platform. 

## 2. Terminology

What follows is a description of the terms that will be encountered the most throughout this document:

* **System**: the complete system architecture, front-end and back-end
* **User**: client who uses the system and can make orders
* **Site**: website
* **Password** and **Username**: credentials used by the user to authenicate himself

## 3. Item Tested

Items that will be tested during this session:

* Ability for a user to access the platform via username and password  
_Test case: 2.1_
* Ability of the system to manage an failed login due to invalid credentials  
_Test cases: 2.2, 2.3_
* Ability of the system to manage purchases  
_Test cases: 2.4, 2.5_
* Ability of the system to manage redeems
_Test cases: 2.6, 2.7_

## 4. Approach

The tests will be conducted manually and offline in order to ensure that the system won't be corrupted nor manipulated in the meanwhile.  
Some features will be tested together but in different test cases, for example the ability of the system to correctly manage purchases.

## 5. Items Pass & Fail Criteria

User backtest will be crucial in order to meet the requirements, so in order to be considered valid a feature has to be easy to use for the user and, most importantly, has to work properly.  
In the opposite case, when a feature doesn't accomplish its goals ot the user is not able to easily use ir, it will be considered as a fail.
