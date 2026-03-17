FROM python:3-slim

WORKDIR /app

COPY . .

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 1080

CMD python3 proxy/tg_ws_proxy.py --host 0.0.0.0 --username ${USERNAME} --password ${PASSWORD}
