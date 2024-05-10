# FastAPI Social Media Backend Project Overview

## Project Features

- **Post Route:** 
  - Creating, deleting, updating, and retrieving posts.
  - CRUD (Create, Read, Update, Delete) operations on posts.
  
- **Users Route:** 
  - User creation and retrieval by ID.
  - Endpoints for creating new users and fetching user details.

- **Auth Route:** 
  - User authentication system for login.
  - Authentication for accessing protected endpoints.

- **Vote Route:** 
  - Voting or liking system for posts.
  - Endpoints for upvoting (no logic for down voting).

## Tech Stack

- **Python:** Primary programming language.
- **FastAPI:** Web framework for high performance.
- **PostgreSQL:** SQL database for user and post data.
- **SQLAlchemy:** ORM tool for database interaction.

## Project Development

1. **Initial Setup:**
   - Development environment setup.
   - Dependency management using virtual environments.

2. **API Development:**
   - Creation of FastAPI routes and endpoints.
   - Implementation of CRUD operations for posts and users.

3. **Database Integration:**
   - Integration of PostgreSQL database.
   - Use of SQLAlchemy for ORM operations.

4. **Authentication and Security:**
   - Implementation of JWT token-based authentication.
   - Password hashing for user security.

   **(To be done)**

5. **Testing and Validation:**
   - Writing unit tests for endpoint reliability.
   - Data validation using schemas and models.

6. **Deployment:**
   - Deployment on various platforms.
   - CI/CD pipelines setup using GitHub Actions.

7. **Documentation:**
   - Utilization of FastAPI's built-in documentation feature.
   - Documentation of API endpoints, schemas, and models.

# How to run locally

### First clone this repo by using following command


`> git clone https://github.com/vishalbansal28/FastAPI-Social-media-backend-clone.git`

`> cd fastapi-course`

##### #### Then install fastapp using all flag like


`pip install fastapi[all]`

##### #### ### Then go this repo folder in your local computer run follwoing command


`uvicorn main:app --reload`

##### ##### Then you can use following link to use the API


> http://127.0.0.1:8000/docs 

##### After run this API you need a database in postgres
##### Create a database in postgres then create a file name .env and write the following things in you file

DATABASE_HOSTNAME = localhost
DATABASE_PORT = 5432
DATABASE_PASSWORD = passward_that_you_set
DATABASE_NAME = name_of_database
DATABASE_USERNAME = User_name
SECRET_KEY = 09d25e094faa2556c818166b7a99f6f0f4c3b88e8d3e7 
ALGORITHM = HS256
> DATABASE_HOSTNAME = localhost
DATABASE_PORT = 5432
DATABASE_PASSWORD = passward_that_you_set
DATABASE_NAME = name_of_database
DATABASE_USERNAME = User_name
SECRET_KEY = 09d25e094faa2556c818166b7a99f6f0f4c3b88e8d3e7 
ALGORITHM = HS256
ACCESS_TOKEN_EXPIRE_MINUTES = 60(base)ACCESS_TOKEN_EXPIRE_MINUTES = 60(base)

**Note: SECRET_KEY in this exmple is just a psudo key. You need to get a key for youself and you can get the SECRET_KEY from fastapi documantion**
