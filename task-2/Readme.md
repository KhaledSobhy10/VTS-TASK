# Task 02 


### Database : No changes to the schema , just add a new record to the status table.

### Request state machine :
![enter image description here](https://github.com/KhaledSobhy10/VTS-TASK/blob/main/task-2/request-state-machine.drawio.png?raw=true)


### Flow charts : 
#### Cancel 
![enter image description here](https://github.com/KhaledSobhy10/VTS-TASK/blob/main/task-2/cancel.flow-chart.png?raw=true)

#### Withdraw 
![enter image description here](https://github.com/KhaledSobhy10/VTS-TASK/blob/main/task-2/withdraw.flow-chart.png?raw=true)

#### Edit pending request
![enter image description here](https://github.com/KhaledSobhy10/VTS-TASK/blob/main/task-2/edit-pending-request.flow-chart.png?raw=true)


### Sequence Diagram :
#### Cancel ![enter image description here](https://github.com/KhaledSobhy10/VTS-TASK/blob/main/task-2/cancel-request-sequance.png?raw=true)

### Withdraw 
![enter image description here](https://github.com/KhaledSobhy10/VTS-TASK/blob/main/task-2/withdraw-request-sequance.drawio.png?raw=true)

#### Edit pending request
![enter image description here](https://github.com/KhaledSobhy10/VTS-TASK/blob/main/task-2/edit-pending-sequance.drawio.png?raw=true)


![enter image description here](https://github.com/KhaledSobhy10/VTS-TASK/blob/main/task-2/manager-page.png?raw=true)


### Pseudocode

    // Cancel approved request
    Employee enter sys after login 
    show requests 
    click approved request  
    if ( date in future && confirmed)
    return updated requests
    else if ( date in last 5 days && confirmed)
    take short explanation from employee then cancel and return new data


    // widthdraw request
    Employee enter sys after login 
    show requests 
    click pedning request  
    if (confirmed)
    return updated requests
    else return to home screen 
    
    // edit pending request
    Employee enter sys after login 
    show requests 
    click pedning request
    employee update data   
    if (confirmed && validate data )
    return updated requests
    else if ( not valid data )
	  return error messages 
    else return to home screen 

		 	 
			    
