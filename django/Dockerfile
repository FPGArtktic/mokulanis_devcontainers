FROM debian:bullseye
RUN  export DEBIAN_FRONTEND=noninteractive

EXPOSE 8000

RUN apt -y update
RUN apt -y upgrade
RUN apt -y install python3 python3-pip build-essential
RUN pip install Django
RUN apt clean 


ENTRYPOINT ["python3"] 
CMD ["/usr/share/nginx/html/mysite/manage.py", "runserver", "localhost:8000"]

