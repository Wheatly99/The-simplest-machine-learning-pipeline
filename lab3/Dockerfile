FROM python:3.10
EXPOSE 8501
WORKDIR /app
COPY requirements.txt ./requirements.txt
RUN pip3 install -r requirements.txt
COPY ../data_creation.py .
COPY ../model_preparation.py .
COPY ../model_preprocessing.py .
COPY ../model_testing.py .
COPY ../pipeline.sh .
CMD ./pipeline.sh

