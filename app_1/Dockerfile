FROM python:3.10-slim

WORKDIR .
COPY ./requirements.txt ./requirements.txt
RUN pip install --no-cache-dir --upgrade -r /requirements.txt ;

COPY . .
ENTRYPOINT uvicorn app:app --host 0.0.0.0 --reload --port 80