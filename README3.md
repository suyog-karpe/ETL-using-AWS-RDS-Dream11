Extract from the Database you have created on AWS-RDS
Use the Following Steps for Exporting from AWS-
1)!pip install mysql.connector
  import mysql.connector
2)conn = mysql.connector.connect(host='database-1.codzmntflx6t.ap-northeast-1.rds.amazonaws.com',user='xxxx',password='*****',database='@name')
  **Note: user: and pasword: should be of the database that you have uploaded.
  The above link of the host is an example of the url that you will find on the Database(endpoint).
  Please make sure the Database name is correct.
3)import pandas as pd
4) delivery = pd.read_sql_query('SELECT * FROM delivery',conn)
  player = pd.read_sql_query('SELECT * FROM player',conn)
  player_captain = pd.read_sql_query('SELECT * FROM player_captain',conn) 





FOR UPLOADING DATA ON AWS-RDS-
1)!pip install mysql.connector
  import mysql.connector
  !pip install pymysql
  import pymysql
  from sqlalchemy import create_engine

2)conn = mysql.connector.connect(host='database-1.codzmntflx6t.ap-northeast-1.rds.amazonaws.com',user='****',password='88888')
3)mycursor =conn.cursor()
4)mycursor.execute('CREATE DATABASE ****')
5)conn.commit()
6)engine = create_engine("mysql+pymysql://user:password@database-olap.cziu2iwkal43.eu-north-1.rds.amazonaws.com/8888(url)")
  export_df.to_sql('batter_points', con = engine)
