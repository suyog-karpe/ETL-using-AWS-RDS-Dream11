Create an Account on AWS you will have to use Credit Card/Debit Info dont worry though such amount is refunded in 3-5 buisness days.
After that move on to console which is your main page where all services are provided <br>
Go to services-->database-->RDS<br>
Click on Create Database<br>
Standered create-> MySQL<br>
Disable RDS Extended Support<br>
Choose->Free Template <br>
create a DB cluter identifier any name eg: database-1<br>
Make sure you turn off any additional payment servives and dont swith from default settings.<br>
Create user(name):eg-admin or root and password.<br>
<br>
<br>
After creating database click on it goto Scroll down Go to VPC Security groups<br>
Click on the big number go down click on inbound rules edit inbound rules<br>
Change type --> all traffic<br>
Change IPversion --IPv4<br>
Do same but cange IPversion ti IPv6 for next one now u have 3 Inbound rules which makes connections with all three categories possible.<br>
Now we are good to go for the next step of extraction and Deletion.<br>
Thankyou!
