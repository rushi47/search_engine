FROM python:3.8-slim-buster
COPY . /app
WORKDIR /app
RUN apt-get -y update && apt-get install -y libzbar-dev
RUN pip install -r requirements.txt
EXPOSE 8501
ENTRYPOINT ["streamlit","run"]
CMD ["app.py"]
