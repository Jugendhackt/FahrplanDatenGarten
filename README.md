![](https://jhbadge.com/?evt=ber&year=2019)

# FahrplanDatenGarten
We  ❤️  Deutsche Bahn
## Features
-
-
-

## Contributors
- [n0emis](https://github.com/n0emis)
- [FänselMänsel](https://github.com/fanselMansel)
- [CodeDoctorDE](https://github.com/CodeDoctorDE) / [Gitlab](https://gitlab.com/CodeDoctorDE)
- [Anna](https://github.com/maedchenkunst2013)
- [LabCode](https://github.com/labcode-de)
## Used API's
  - HAFAS
# Develeopment Setup



## Set up the VEnv:
```
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```
## Set up the database:
Change the `DATABASE_URL` in `.env` basend on the `.env.example` and https://github.com/jacobian/dj-database-url.
Now run
```
source .env
python manage.py migrate
```

## Import Stations from DB
```
python manage.py dbapis_importstations
```

## Import Timetable from DB
```
python manage.py dbapis_timetable {IfOpt}
```

## Start Webserver
```
python manage.py runserver
```
The Webserver now runs under http://127.0.0.1:8000/verspaeti/

## Themes

There are four different themes to choose from:
* Dark (`@import './styles/dark'`)
* Dark-Mixed (`@import './styles/dark-mixed'`)
* Light (`@import './styles/light'`)
* Light-Mixed (`@import './styles/light-mixed'`)

Change the imports in the `frontend/style.sass` and compile sass!
