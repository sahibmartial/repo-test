FROM python:2.7-stretch
MAINTAINER Martial(sahibkonan@gmail.com)
# update and install flask
RUN apt-get update -y && apt-get install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y
RUN pip install flask flask_httpauth flask_simpleldap python-dotenv

#create volume
RUN mkdir /data
#copy source
COPY student_age.py .
#port
EXPOSE 5000
#run cmd
CMD [ "python", "./student_age.py" ]



