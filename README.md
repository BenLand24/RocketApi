https://rocket-restapi.herokuapp.com/api/employees need to get endpoint for email

https://rocket-restapi.herokuapp.com//api/interventions/ to get elevator id in pending status

------------------------------------------------------------------

Rocket Elevators REST API URL: https://rocket-restapi.herokuapp.com//api

How to answer the 3 requests in Postman :

1- To get the interventions that have a pending status and no start date, you do :

GET https://rocket-restapi.herokuapp.com//api/intervention	
SEND
2- If you wish to see a specific intervention, you do :

GET https://rocket-restapi.herokuapp.com//api/intervention/id		[5 = specified battery ID]
SEND
3- To modify the status to "in progress" and change the start date to right now, you do :

PUT https://rocket-restapi.herokuapp.com//api/intervention/id/inProgress  [5 = specified column ID]
SEND
Select:  Body
            Raw
            JSON application
You should see a message confirming that the change has been done.

4- To modify the status to "completed" and change the start date to right now, you do

PUT https://rocket-restapi.herokuapp.com//api/intervention/id/completed [5 = specified column ID]
SEND
An error will appear in the field, that's ok.
Select:  Body
            Raw
            JSON application
You should see a message confirming that the change has been done.

5- To verify by yourself that the statuses have been changed, repeat step 2 with the id number.
