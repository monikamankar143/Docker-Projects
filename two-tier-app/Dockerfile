FROM python:3.9-slim

RUN apt-get update \
    && apt-get upgrade -y \
    && apt-get install -y gcc default-libmysqlclient-dev pkg-config \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /app

COPY . .

# Install app dependencies
RUN pip install --upgrade pip \
    && pip install mysqlclient \
    && pip install -r requirements.txt


# Specify the command to run your application
CMD ["python", "app.py"]
