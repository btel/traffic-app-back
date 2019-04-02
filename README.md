To run the unit tests you will need to install a postgres and create a database called `traffictestdb` with your current user.

# Depolying

## Seed database


Initialize database:

```
heroku run 'FLASK_APP=traffic_back flask init-db'
```

Import data:

```
DATABASE_URL="postgresql://url_to_your_heroku_postgress" FLASK_APP=traffic_back flask import-traffic PATH_TO_CSV_DATA
```
