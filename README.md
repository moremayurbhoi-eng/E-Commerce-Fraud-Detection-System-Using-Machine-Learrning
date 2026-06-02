# E-Commerce-Fraud-Detection-System-Using-Machine-Learrning

1. Start MySQL Server

Open MySQL Workbench or Services and make sure MySQL is running.

2. Create Database
CREATE DATABASE frauddetectionml;
3. Import Database

If you have an SQL file:

Open MySQL Workbench
Select frauddetectionml
Go to Server → Data Import
Choose your .sql file
Click Start Import
4. Open Project Folder

Open Command Prompt or Anaconda Prompt:

cd project_folder_path

Example:

cd D:\Projects\EcommerceFraudDetection
5. Create Virtual Environment (Optional)
python -m venv venv

Activate:

venv\Scripts\activate
6. Install Required Libraries
pip install flask pymysql pandas numpy scikit-learn joblib

Or:

pip install -r requirements.txt
7. Configure Database Connection

In app.py find:

conn = pymysql.connect(
    host="localhost",
    user="root",
    password="your_password",
    database="frauddetectionml"
)

Update with your MySQL password.

8. Run the Project
python app.py

If successful, you will see:

* Running on http://127.0.0.1:5000
9. Open Browser

Visit:

http://127.0.0.1:5000
