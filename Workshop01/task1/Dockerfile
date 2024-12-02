FROM python:3.9-slim 

LABEL maintenance=Ricky
LABEL task=day1_workshop01_task1

ENV FLASK_RUN_HOST=0.0.0.0

ENV INSTANCE_NAME="" \
    INSTANCE_HASH="" \
    PORT=3000

WORKDIR /app

COPY . /app

RUN pip install --no-cache-dir flask

EXPOSE 3000

CMD ["sh", "-c", "python main.py --port=${PORT} --name=${INSTANCE_NAME} --hash=${INSTANCE_HASH}"]

