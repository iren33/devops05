FROM python:3.8.5     
 
ADD hits /devops05/hits/
WORKDIR /devops05

COPY requirements.txt .
RUN apt-get  update 
RUN apt-get install python3-pip -y 
RUN pip3 install -r requirements.txt
RUN mkdir /devops05/logs
  
 
CMD ["hits/app.py"] 

EXPOSE 5000
