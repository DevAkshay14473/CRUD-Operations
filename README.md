# CRUD-Operations
 create a shopping cart by python REST API using flask and mysql that handles CRUD operations for a specific user
from flask import Flask

app = Flask(__name__)

from app import app
from flaskext.mysql import MySQL

mysql = MySQL()
 
# MySQL configurations
app.config['MYSQL_DATABASE_USER'] = 'root'
app.config['MYSQL_DATABASE_PASSWORD'] = 'root'
app.config['MYSQL_DATABASE_DB'] = 'roytuts'
app.config['MYSQL_DATABASE_HOST'] = 'localhost'
mysql.init_app(app)
