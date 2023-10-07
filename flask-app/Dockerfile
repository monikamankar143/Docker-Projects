#Create base image
FROM python:3.9

#Working directory for the app
WORKDIR app/

#Copy the copy from system to current directory
COPY app.py .

#Install the required libraries
RUN pip install flask

#Run the appllication
CMD ["python","app.py"]

