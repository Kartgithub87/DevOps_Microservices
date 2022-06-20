FROM python:3.7.3-stretch

# Working Directory
WORKDIR /app

# Copy source code to working directory
COPY . flask_app/web.py /app/
COPY . nlib /app/

# Install packages from requirements.txt
# hadolint ignore=DL3013
RUN pip install  --no-cache-dir --upgrade pip &&\
    pip install --trusted-host pypi.python.org  --no-cache-dir -r requirements.txt
    
EXPOSE 80   

CMD python3 ./web.py