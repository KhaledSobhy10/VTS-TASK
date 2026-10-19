# A Vacation Tracking System

## 1- Vision 
A Vacation Tracking System (VTS) will provide individual employees with the capability to manage their own vacation time, sick leave, and personal time off, without having to be an expert in company policy or the local facility’s leave policies, **The system must be easy to use.** 
 
 ## 2- Domain ( Problem ) 
 The Problem Managing leave requests is difficult and slow for employees, managers, and HR :
  - Employees struggle to view their leave balance and request status.
 - Managers find it hard to approve requests or directly grant leave time.
  - Tracking leave requests manually becomes hard as the company grows.
 
## 3- Functionl Requirements
- Employee can sign in and request vacation
- Enables manager approval (optional)
- Provides access to requests for the previous calendar year, and allows requests to be 		  made up to a year and a half in the future 
- Uses e-mail notification to request manager approval and notify employees of request status changes 
- Keeps activity logs for all transactions 
- Enables the HR and system administration personnel to override all actions restricted by rules, with logging of those overrides 
- Allows managers to directly award personal leave time (with system-set limits)
- Provides a Web service interface for other internal systems to query any given employee’s vacation request summary 
- Interfaces with the HR department legacy systems to retrieve required employee information and changes
- Interface as web application  for end users ( HR , Managers , Employees )

## 4- Non-Functional  Requirements
- Employees should be able to submit a leave request with minimum steps .

## 5- Constraints
-  **Internal Network:** Must operate strictly within the corporate **intranet**.
- **Integration :** Must integrate with the existing user **authentication system** and another legacy systems .
- **Tech Stack:** May be use the **pre-selected** technology stack.

## 5- Actors 

|Actor  | Actions|
|--|--|
|**Manager**| Approve , Reject and Award time |
|**Clerk (HR)** | Edit employee record , define leave category , overried leave record and manage locations|
|**Employee**| Manage leave| 
|**System Admin**| Back up system logs |


## 6- Use-case ( mange time )

>  Manage Time: Describes how employees request and view vacation time
> requests.

### 6.1 Entities (Data Model) 


![### Entities](https://raw.githubusercontent.com/KhaledSobhy10/VTS-TASK/refs/heads/main/entities.drawio.png)


### 6.2 flow-chart
![flow chart](https://raw.githubusercontent.com/KhaledSobhy10/VTS-TASK/refs/heads/main/flowchart.png)


### 6.3 Pseudocode

BEGIN
    Employee logs in to the system

    OPEN Manage Time sys

    DISPLAY "1. Request Vacation"
    DISPLAY "2. View Vacation Requests"

    INPUT choice

    IF choice = 1 THEN

        INPUT start_date
        INPUT end_date
        INPUT reason

        IF vacation dates and information are valid THEN

            SAVE vacation request

            DISPLAY "Vacation request submitted successfully"

        ELSE
            DISPLAY "Error: Invalid request"
        END IF

    ELSE IF choice = 2 THEN

        DISPLAY vacation requests
        DISPLAY request status

    ELSE

        DISPLAY "Invalid choice"

    END IF

### 6.4 sequence diagram
	![enter image description here](https://raw.githubusercontent.com/KhaledSobhy10/VTS-TASK/refs/heads/main/sq-digram.drawio.png)
