FROM python:slim
WORKDIR /app
COPY requirements.txt requirements.txt
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
RUN chmod +x docker-entrypoint.sh
VOLUME [ "/app/data" ]
ENTRYPOINT [ "./docker-entrypoint.sh" ]
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]