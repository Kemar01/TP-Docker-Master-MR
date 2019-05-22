FROM centos
RUN yum update -y && yum install httpd  python python-flask python-requests sudo -y 
EXPOSE 8001
RUN echo 'Hello' /var/www/html/index.html
RUN service httpd restart
ADD /TP-Docker-master/api-backend/api.py /
RUN python api.py
