FROM python:3.8

WORKDIR /app

COPY requirements.txt ./

RUN pip install -r requirements.txt

COPY . .

CMD ["python", "test.py"]

# docker build -t test_image . ; docker run -it --rm test_image; docker rmi test_image
