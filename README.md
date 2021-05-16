## Mini-project - Make a flask api secure with JWT token and authentication

## Stack

- Api: image: python:slim-3.9
- Database: Sqlite3

## Sample small project
Users & Authors. Database file called library.db.

## Getting started

```
docker-compose up -d
```

Once, library.db created
```
sudo chown -R $USER:$USER .
```

### SQLite commands
```
docker-compose run --rf sqlite3 sqlite3 library.db
```

#### CommandLine - databases
```
.databases
```
#### CommandLine - tables
```
.tables
```

### Api commands
```
docker-compose exec api python3
```

#### Create tables - python

```
>>> from main import db
>>> db.create_all()
```
