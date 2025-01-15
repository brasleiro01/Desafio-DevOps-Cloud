FROM python:3.9.21-slim
WORKDIR /app
COPY requirementes.txt .
RUN pip install --upgrade pip
RUN pip install -r requirementes.txt
COPY . /app/
EXPOSE 5000
CMD [ "gunicorn", "--bind", "0.0.0.0:5000", "app:app" ]