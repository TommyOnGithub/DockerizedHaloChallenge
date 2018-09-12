FROM python:2.7.10
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
COPY requirements.txt /usr/src/app/
RUN pip install --upgrade pip
RUN pip install --no-cache-dir --trusted-host pypi.python.org -r requirements.txt
RUN pip install --no-cache-dir --trusted-host pypi.python.org psycopg2-binary
COPY . /usr/src/app
