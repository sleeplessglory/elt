FROM python:3.8-slim
#install PostgreSQL with some command line tools
RUN apt-get update && apt-get install -y postgresql-client
#copy the contents of the ELT script (so, the Docker container has access to it)
COPY elt_script.py .

CMD ["python", "elt_script.py"]