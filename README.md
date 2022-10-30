# CrowdFunding

**CrowdFunding** is an Egyptian for-profit crowd funding platform that allows people to raise money for events ranging from life events such as celebrations and graduations to challenging circumstances like accidents and illnesses.
The project is developed using **Python**, **Django** framework and **MySQL** database.


## Deployment

---

https://crowd-funding-web.herokuapp.com/


## Table of Contents

---

<!-- TOC -->

- [Features](#features)
- [Getting Started](#getting-started)
  - [Setup Your Environment](#setup-your-environment)
  - [Using Docker](#using-docker)
  <!-- /TOC -->

## Features

---

- Sign in with your Google / Facebook accounts
- Create a fund raising campaign
- Report campaigns
- Rate campaigns
- Add comments to any campaign
- Reply to comments
- Report comments
- View all your campaigns and donations
- Live search for campaigns 
- Browse campaigns based on category

## Getting Started

---

To use and run this project you need to:

Before executing the following commands, please install python 3 as stated in the following setup


#### Setup Your Environment

---

1. Run the following command to install the project locally.

```bash
python3 -m pip install --upgrade pip

git clone https://github.com/khaledabotaleb/Crowd-Funding.git

cd crowd-funding-django/ 

python3 -m venv venv

source venv/bin/activate

pip3 install -r requirements.txt 
```

2. Execute configuration required in configurations section

```bash
python3 manage.py migrate
```

3. Run the server

```
python3 manage.py runserver
```

4. Go to the browser and go to the following url: **http://127.0.0.1:8000**

##### Note:

Make sure that your database is up and configured properly for the application to work

#### Using Docker

---

You can also use the docker image provided to setup a running environment
for the application to avoid any environment conflicts.

Change your working directory to the projects folder and execute the following commands (only one time)

```bash
docker-compose build
```

to build the image and then

```bash
docker-compose run app python3 manage.py migrate
```



