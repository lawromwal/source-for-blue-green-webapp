FROM 822580616975.dkr.ecr.us-east-1.amazonaws.com/capstone-base-image

RUN apk add python3 py-pip && \
python3 -m ensurepip && \
pip install --upgrade pip && \
pip install flask

ENV FLASK_APP app.py
ENV PLATFORM 'Amazon EKS'

WORKDIR /app
COPY . /app/

CMD ["python", "app.py"]
