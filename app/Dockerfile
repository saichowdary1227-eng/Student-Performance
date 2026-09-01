FROM python:3.12
WORKDIR /student
COPY app/requirements.txt .
RUN pip install -r app/requirements.txt
COPY . .
RUN python3.12 app/train.py
EXPOSE 5000
CMD ["python3.12", "app/app.py"]
