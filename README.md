
# Task_Fastapi_project 



a project to take and return task for a crawler server and manage datas 

also generate and return response with graphql server to access any data you need 


this app can handle something like:

1.crud request to done with crawler server 

2.assign task to crawler 

3.get response from crawler and save 


!! make sure to install postgresql and mongodb on your system 

for run server first you need to run this command 
``pip install -r requirements``

to migrate and make database run this command 

`` alembic revision --autogenerate -m "create job model"
alembic upgrade head ``

then run   ``main.py `` file and open ``127.0.0.1:8000/docs/``

or if you have docker or docker-compose on your systems you can run this command instead 
```docker-compose up -d --build ``` or with docker :
```docker build -t  your_image_name:tag .```
```docker run -d your_container_name -p 8000:8000 -p 7000:7000 your_image_name:tag```

consider to have mongodb and postgres_db on your local pc when you wanna to run with command 
or run with docker file 

you need to have mongodb on your pc and put the correct value on file 
`models/model_explore` to save datas 
