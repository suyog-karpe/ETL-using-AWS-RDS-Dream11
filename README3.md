### Extract from the Database you have created on AWS-RDS
Use the Following Steps for Exporting from AWS-
1)!pip install mysql.connector<br>
  import mysql.connector<br>
2)conn = mysql.connector.connect(host='database-1.codzmntflx6t.ap-northeast-1.rds.amazonaws.com',user='xxxx',password='*****',database='@name')<br>
  **Note: user: and pasword: should be of the database that you have uploaded.<br>
  The above link of the host is an example of the url that you will find on the Database(endpoint).<br>
  Please make sure the Database name is correct.<br>
3)import pandas as pd<br>
4) delivery = pd.read_sql_query('SELECT * FROM delivery',conn)<br>
  player = pd.read_sql_query('SELECT * FROM player',conn)<br>
  player_captain = pd.read_sql_query('SELECT * FROM player_captain',conn)<br>


<br>
<br>


### FOR UPLOADING DATA ON AWS-RDS-
1)!pip install mysql.connector<br>
  import mysql.connector<br>
  !pip install pymysql<br>
  import pymysql<br>
  from sqlalchemy import create_engine<br>

2)conn = mysql.connector.connect(host='database-1.codzmntflx6t.ap-northeast-1.rds.amazonaws.com',user='****',password='88888')<br>
3)mycursor =conn.cursor()<br>
4)mycursor.execute('CREATE DATABASE ****')<br>
5)conn.commit()<br>
6)engine = create_engine("mysql+pymysql://user:password@database-olap.cziu2iwkal43.eu-north-1.rds.amazonaws.com/8888(url)")<br>
  export_df.to_sql('batter_points', con = engine)<br>
