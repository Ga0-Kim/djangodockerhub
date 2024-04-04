FROM python

WORKDIR /usr/src/app
COPY requirements.txt ./
RUN pip install -r requirements.txt
COPY . .

EXPOSE 80
# 파이썬 프로젝트는 이부분만 변경
CMD ["python", "manage.py", "runserver", "0.0.0.0:80"]