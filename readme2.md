Create an Account on AWS you will have to use Credit Card/Debit Info dont worry though such amount is refunded in 3-5 buisness days.
After that move on to console which is your main page where all services are provided 
Go to services-->database-->RDS
Click on Create Database
Standered create-> MySQL
Disable RDS Extended Support
Choose->Free Template 
create a DB cluter identifier any name eg: database-1
Make sure you turn off any additional payment servives and dont swith from default settings.
Create user(name):eg-admin or root and password.


After creating database click on it goto Scroll down Go to VPC Security groups
Click on the big number go down click on inbound rules edit inbound rules
Change type --> all traffic
Change IPversion --IPv4
Do same but cange IPversion ti IPv6 for next one now u have 3 Inbound rules which makes connections with all three categories possible.
Now we are good to go for the next step of extraction and Deletion.
Thankyou!
