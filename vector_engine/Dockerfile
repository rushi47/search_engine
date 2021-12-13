FROM python:3.8-buster
COPY . /app
WORKDIR /app
RUN apt-get -y update && apt-get install -y libzbar-dev && apt-get install -y rustc gcc swig
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
EXPOSE 8501
ENTRYPOINT ["streamlit","run"]
CMD ["app.py"]
