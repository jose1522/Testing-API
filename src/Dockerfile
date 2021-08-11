FROM python:latest
RUN mkdir /app
WORKDIR /app
ADD . /app
RUN echo "Debugging - Root files"
RUN ls
RUN echo "Debugging - App files"
RUN ls /app
RUN pip install --upgrade pip setuptools wheel
RUN pip install -r requirements.txt
EXPOSE 8080
CMD ["uwsgi", "app.ini"]