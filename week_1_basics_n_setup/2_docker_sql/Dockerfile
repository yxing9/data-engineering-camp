FROM python:3.11

# RUN pip install pandas
RUN apt-get install wget
RUN pip install pandas sqlalchemy psycopg2

WORKDIR /app
# COPY pipeline.py pipeline.py
COPY ingest_data.py ingest_data.py 

# ENTRYPOINT [ "bash" ]
# ENTRYPOINT [ "python", "pipeline.py" ]
ENTRYPOINT [ "python", "ingest_data.py" ]