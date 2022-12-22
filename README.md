# Casting Agency Capstone Project

This is my final capstone project for Udacity's FullStack Web Developer Nanodegree.
Web app can be accessed at [here](https://capstonenhatmq.herokuapp.com)

### Project Dependencies
* __Python 3.10__ - Follow instructions to install the latest version of python for your platform in the [python docs](https://docs.python.org/3/using/unix.html#getting-and-installing-the-latest-version-of-python)
* __Flask__ - Slim python web library.
* __SQLAlchemy__ - Python ORM library
* __Heroku__ - PaaS platform for easy hosting of web apps
* __Postman__ - API testing tool

### Installation instructions
* Clone project to directory of your choice.
* Create a virtualenv in project directory
* run ```pip install -r requirements.txt``` to install project dependencies
* add ```DATABASE_URL``` to environment variables of your system. 
On Unix systems, use ```export DATABASE_URL=postgresql://{username}:{password}@{host}:{port}/{database_name}```
* run ```export FLASK_APP=app.py```
* type ```flask run``` in terminal

### Endpoints:
* GET /actors and /movies
* DELETE /actors/ and /movies/
* POST /actors and /movies and
* PATCH /actors/ and /movies/

### Roles
* Casting Assistant
    * GET /actors and /movies

* Casting Director
    * GET /actors and /movies
    * ADD /actors and DELETE /actors
    * PATCH /actors and /movies
    
* Executive Producer
    * GET /actors and /movies
    * ADD /actors and DELETE /actors
    * PATCH /actors and /movies
    * ADD /movies and DELETE /movies


### JWT Tokens for each role:
* Casting Assistant - ```eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Ijd2SDRyOW5wWUhvd2ktcEg3clVCTiJ9.eyJpc3MiOiJodHRwczovL25oYXRtcS51cy5hdXRoMC5jb20vIiwic3ViIjoiYXV0aDB8NjMwNTM5MGYwNmE0N2M2YWI2YzdhZmIzIiwiYXVkIjoiQ2Fwc3RvbmUiLCJpYXQiOjE2NzIwMDExMDcsImV4cCI6MTY3MjAwODMwNywiYXpwIjoickY1M3A5N1EwT1JoNUFwb21yNmJwNzZQcXhUSXppQWciLCJzY29wZSI6IiIsInBlcm1pc3Npb25zIjpbInZpZXc6YWN0b3JzIiwidmlldzptb3ZpZXMiXX0.kwLDO_Lq6Cs6FbhQvodzhdj_RRISd3f6JRmE9o9semrkEzfdX2Z0G02Fu58KFtEk9yjDcCtlyVuhxEu9mZuRL_SOhb3e05a_UFk1yFtOcT64yilFDo_JMvIxq42yW9IBY67ZMBHt94mxJp2qtx-jW5DMa6viiSdyNWjLT0L5wSIYSkvib55KZ1dF_oj9rh0DvISSz23OI_ZQtirRJhwmLqL4lrWyGWomdkkNWqLxMrX37xGzBkcLe94SNghVjUdo5t5Y75Gn93N3VaAS0pE0i3UqdWfGjtW_meKwzbzWoJesi-Lws-wgowmHuu7DKsclpAZxFIyw6nZ5cN5gUr_q4g```

* Casting Director- ```eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Ijd2SDRyOW5wWUhvd2ktcEg3clVCTiJ9.eyJpc3MiOiJodHRwczovL25oYXRtcS51cy5hdXRoMC5jb20vIiwic3ViIjoiYXV0aDB8NjMwNTM5NDYwNmE0N2M2YWI2YzdhZmM0IiwiYXVkIjoiQ2Fwc3RvbmUiLCJpYXQiOjE2NzIwMDA5OTYsImV4cCI6MTY3MjAwODE5NiwiYXpwIjoickY1M3A5N1EwT1JoNUFwb21yNmJwNzZQcXhUSXppQWciLCJzY29wZSI6IiIsInBlcm1pc3Npb25zIjpbImFkZDphY3RvcnMiLCJkZWxldGU6YWN0b3JzIiwiZGVsZXRlOm1vdmllcyIsInVwZGF0ZTphY3RvcnMiLCJ1cGRhdGU6bW92aWVzIiwidmlldzphY3RvcnMiLCJ2aWV3Om1vdmllcyJdfQ.ZIlQ2hTKAuqC4a7kKv6Nq59jB7U3WTOS6LKJDDn03ZAdnFPRX0R_KhXiq4W2vewWvtWrCHSzUNG_7DTCXJGcLYss-6X7jYjDREYhMCOTxVVgimC-iulnoWIePxbLG724BsBaWf5mnI7vyjvZvXNXSqOg190OHV1Iq3_Smgh3YaTuRO460IbUV7mgWr-NeZ1S0iGdubE6X_isErDw8mFQ1DC6s0z1E2iAfs5Fz9qWNrdJmlKoGNU1XH7wGKsnunJWJO8vkeROECTY4rijKMl1md-pcA-S0LF8XDJ7r3taEw5NxSBMdrn1Xgdyg9SMhc_5qpqW67wlf8CCuZ9nKyWSIw```

* Executive Producer - ```eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Ijd2SDRyOW5wWUhvd2ktcEg3clVCTiJ9.eyJpc3MiOiJodHRwczovL25oYXRtcS51cy5hdXRoMC5jb20vIiwic3ViIjoiZ29vZ2xlLW9hdXRoMnwxMDQ1NzMwNTk5ODgxNzU3MjE3MTAiLCJhdWQiOiJDYXBzdG9uZSIsImlhdCI6MTY3MjAwMTE2NSwiZXhwIjoxNjcyMDA4MzY1LCJhenAiOiJyRjUzcDk3UTBPUmg1QXBvbXI2YnA3NlBxeFRJemlBZyIsInNjb3BlIjoiIiwicGVybWlzc2lvbnMiOlsiYWRkOmFjdG9ycyIsImFkZDptb3ZpZXMiLCJkZWxldGU6YWN0b3JzIiwiZGVsZXRlOm1vdmllcyIsInVwZGF0ZTphY3RvcnMiLCJ1cGRhdGU6bW92aWVzIiwidmlldzphY3RvcnMiLCJ2aWV3Om1vdmllcyJdfQ.cvo2FsUPwpxGg90bCgm6cIuQ5jsSZ3P5LTF7P6LGpZhRRJwjHRQ81oJSGY6bWBGxB4ZEgt00yqaUQinMmKf4lAf8QFwjV-buF_6oPXGIUHu_ekr1kPNxcTKZqYC1Dd0HDzjygig0WL1zAsDkKwVTQ1W0lU9DTP-Tft5ELTpmQ7cHQ--UoqEyL9JW5Li9ndghMzVEZasMcWp3UXGyM7lrAVgWTX0FyURw0jz4D3CoyGs0UdBKVN75McPGv8enXdn8v3o2_KpYAE-8UTxcMrhlFXRbFxLavVgBNmG83NHF0mZD_M66Pm7bzOaIGqowBmtfEvv-RqnlHvCgLakzbMpCTw```

## API Endpoints

In the next few subsections, we'll cover how the API works and what you can expect back in the results.

### Default Path

#### GET /
Verifies that application is up and running on Heroku.

Sample response:
```
{
    "description": "App is running.",
    "success": true
}
```

### GET Endpoints

#### GET /movies
Displays all movies listed in the database.

Sample response:
```
{
    "movies": [
        {
            "id": 3,
            "release_year": 2012,
            "title": "Movie 3"
        },
        {
            "id": 4,
            "release_year": 1956,
            "title": "Movie 4"
        },
    ],
    "success": true
}
```

#### GET /actors
Displays all actors / actresses listed in the database.

Sample response:
```
{
    "actors": [
        {
            "age": 27,
            "gender": "female",
            "id": 3,
            "movie_id": 2,
            "name": "Actor 3"
        },
        {
            "age": 36,
            "gender": "male",
            "id": 4,
            "movie_id": 3,
            "name": "Actor 4"
        },
    ],
    "success": true
}
```

### POST Endpoints

#### POST /movies/create
Creates a new movie entry in the database.

Sample response:
```
{
    "movie_id": 8,
    "success": true
}
```

#### POST /actors/create
Creates a new actor / actress entry in the database.

Sample response:
```
{
    "actor_id": 7,
    "success": true
}
```

### PATCH Endpoints

#### PATCH /movies/update/<movie_id>
Updates movie information given a movie_id and newly updated attribute info.

Sample response:
```
{
    "movie_id": 2,
    "success": true
}
```

#### PATCH /actors/update/<actor_id>
Updates actor information given a actor_id and newly updated attribute info.

Sample response:
```
{
    "actor_id": 2,
    "success": true
}
```

### DELETE Endpoints

#### DELETE /movies/delete/<movie_id>
Deletes a movie entry from the database given the inputted movie_id.

Sample response:
```
{
    "deleted": 1,
    "success": true
}
```

#### DELETE /movies/actors/<actor_id>
Deletes an actor / actress entry from the database given the inputted actor_id.

Sample response:
```
{
    "deleted": 1,
    "success": true
}
```