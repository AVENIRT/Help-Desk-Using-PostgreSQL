# Help-Desk-Using-PostgreSQL
We are now working with a database which notes helpdesk action.  

There are two tables.  First, there is the employee table, which contains the employee’s ID as the primary key, first name, last name, and location.  You can assume all employees at our company are listed here.

Second, there is the ticket table, which contains each individual helpdesk ticket.  The ticket table contains the ticket ID as the primary key, a description of the helpdesk incident, the duration in minutes, a priority, a status, and which employee (if any) has been assigned to the ticket.  If nobody is available, a ticket will be logged into the system in this table, but no employee will be assigned yet.    

The incident status can be completed, in progress, or not started.  If an incident is completed, the duration field will contain the number of minutes the incident took and the employee ID will reference the employee who completed the service.  

If an incident is in progress, the duration field number denotes the number of minutes since the incident started and the employee ID will reference the employee who is currently working on the service (assume for now that all incidents will be completely serviced by the single employee who is assigned to them.)

If an incident service is not yet started, the duration field will be blank, and there will not be an employee assigned to that incident, either.
