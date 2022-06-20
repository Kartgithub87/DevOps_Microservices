FROM python:3.7.3-stretch
LABEL maintainer="Udacity"

WORKDIR /app

COPY . app.py /app/

RUN pip install  --no-cache-dir --upgrade pip &&\
    pip install --trusted-host pypi.python.org  --no-cache-dir -r requirements.txt

# command to run on container start
CMD ["python", "./app.py"]
