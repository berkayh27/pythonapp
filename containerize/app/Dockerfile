FROM python:3

COPY . /app
WORKDIR /app

ENV ENVIRONMENT=docker
ENV FLASK_APP=/app/src/server.py
ENV FLASK_DEBUG=0

RUN pip install -r /app/src/requirements.txt

EXPOSE 8000 

CMD ["python", "-u", "-m", "flask", "run", "--no-reload", "--port", "8000", "--host", "0.0.0.0"]