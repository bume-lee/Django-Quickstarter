# Django-Quickstarter

[![Updates](https://pyup.io/repos/github/sirrobot01/django-quickstarter/shield.svg)](https://pyup.io/repos/github/sirrobot01/django-quickstarter/)
[![Python 3](https://pyup.io/repos/github/sirrobot01/django-quickstarter/python-3-shield.svg)](https://pyup.io/repos/github/sirrobot01/django-quickstarter/)

## 구성

- Custom user
- Authentication(JWT) with Registration
- Requirements file
- Django REST framework
- API Documentations(Swagger & Redoc)
- Django CORS headers

## Installation

venv생성 및 django설치

```bash
mkdir newproject && cd $_
python3 -m venv venv
source venv/bin/activate
pip3 install django==1.11
```

프로젝트 생성

```bash
django-admin startproject --template https://github.com/bume-lee/django-quickstarter/archive/master.zip repo
```

requirements.txt 파일에서 선언된 종속항목 설치

```bash
pip3 install -r requirements.txt
```


마이그레이션 파일 생성 및 적용

```bash
python manage.py makemigrations
python manage.py migrate
```


## API

##### Authentications

- Register `POST` `/auth/register/`
- Login `POST` `/auth/login/`
- Refresh JWT Token `POST` `/auth/refresh/`
- Verify JWT Token `POST` `/auth/verify/`


##### Documentations

- Swagger `GET` `/swagger`
- Redoc `GET` `/redoc/`

## 실행 테스트

```bash
python manage.py test
```
