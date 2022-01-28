FROM python:3.8.2

# init
RUN apt-get update
RUN apt-get upgrade -y
RUN pip install -U pip
RUN apt-get install -y git

# pip
WORKDIR /tmp
COPY requirements.txt .
RUN pip install -r requirements.txt

# clean
RUN rm -rf /var/lib/apt/lists/*