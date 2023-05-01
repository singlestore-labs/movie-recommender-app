FROM python:3.9.16
ENV STATIC_URL /static
ENV STATIC_PATH /var/www/app/static
ENV FLASK_APP /var/www/app/main.py
COPY ./requirements.txt /var/www/requirements.txt
COPY . /var/www/app/
RUN pip install -r /var/www/requirements.txt
CMD ["python3", "-m" , "flask", "run", "--host=0.0.0.0"]