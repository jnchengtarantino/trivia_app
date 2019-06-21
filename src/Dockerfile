FROM python:3.7.3-alpine3.9
LABEL maintainer "John-Nicholas Cheng-Tarantino <jn@chengtarantino.com>"
RUN apk update
RUN mkdir /app
COPY . /app
WORKDIR /app
RUN pip install --no-cache-dir -r requirements.txt
RUN chmod 644 app.py
CMD ["python", "app.py"]
EXPOSE 5000