FROM python
ENV PYTHONBUFFERED 1 
COPY requirements.txt .
RUN apt update \
    && apt upgrade -y \
    && apt install apt-utils -y 
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
RUN mkdir /code
COPY code /code/
WORKDIR /code
