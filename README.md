# Project name: data_engineering_project_openweathermap_api_airflow_etl_aws
Technology used:
+ Virtual environment: Amazon EC2(Apache airflow)
+ Programming language: Python
+ Data Lake: Amazon S3
+ Tool: Vs Code
## Create a virtual machine on EC2
![image](https://github.com/user-attachments/assets/fd77b920-7f9b-4dc7-9c6c-12ca5d13f3c8)
Commands used in this EC2 instance
```sudo apt update
   sudo apt install python3-pip
   sudo apt install python3-venv
   python3 -m venv airflow_venv
   source airflow_venv/bin/activate
   pip install pandas
   pip install s3fs
   pip install apache-airflow
   airflow standalone
   pip install awscli
   aws configure
   aws sts get-session-token
```
## Connect VSCode to EC2 via SSH with the following syntax:
Connect to Visual Studio Code

Install extension: remote ssh

configuration ssh
```
Host weatherApiAirflow
    HostName 54.206.202.44
    User ubuntu
    IdentityFile /Users/hunglo/Downloads/weather-api-airflow-yml.pem
Put command chmod 400 /Users/hunglo/Downloads/weather-api-airflow-yml.pem
ssh -v -i /Users/hunglo/Downloads/weather-api-airflow-yml.pem [ubuntu@](mailto:ubuntu@3.25.62.62)54.206.202.44
```
## Modeling the ETL process
![image](https://github.com/user-attachments/assets/7ba1442b-9715-4c19-966b-4294544e8c3e)
## Result
![image](https://github.com/user-attachments/assets/e6f19d9b-3428-46c8-a3ec-bf9faa2c4a94)
