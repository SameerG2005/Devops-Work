#pulling base image 
FROM python:3.9
#update ubuntu and install git 
RUN apt-get update -y && apt-get install git -y
#working dir to run app
WORKDIR /devops
#get the project source code
RUN git clone https://github.com/LondheShubham153/django-notes-app.git
#install required packages from given path 
RUN pip install -r django-notes-app/requirements.txt
#exposing port where app runs
EXPOSE 8080
#run server of app
CMD ["python","django-notes-app/manage.py","runserver","0.0.0.0:8080"]
