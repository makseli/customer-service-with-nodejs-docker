
# Customer Service with nodejs+docker 

This is a customer service API Backend application. It is powered by NodeJS and Docker and allows you to use different databases (such as MongoDB, PostgreSQL, or MySQL). 

## Key Features:

**Technology Stack**: Node.js, Express.js, MongoDB, MySQL, PostgreSQL

**Containerization**: Docker Compose for development and production environments

**Database Abstraction**: Utilized database service interfaces for MongoDB, MySQL, and PostgreSQL

**Testing**: Implemented comprehensive unit tests using Jest framework

**RESTful API**: CRUD operations for customer management with robust error handling

**Environment Variables**: Managed configuration using dotenv for secure deployment

**Repository Link**: https://github.com/makseli/customer-service-with-nodejs-docker

I invite you to explore the codebase to gain insights into my development practices and methodologies. Feel free to reach out if you have any questions or feedback.

TODO

- [x] Prepare development environment
- [x] Endpoint routing work with Express
- [x] MongoDB implementation
- [x] Posqresql implementation
- [x] Mysql implementation
- [x] Coding test
- [x] Run With Docker-Compose
- [ ] CI/CD entegration
- [ ] Swagger Api Documentation

for mysql create table;
``` sql
CREATE TABLE mydatabase.customers (
	id BIGINT NOT NULL,
	CONSTRAINT p_pk PRIMARY KEY (id),
	name varchar(100) NOT NULL,
	email varchar(100) NOT NULL
)
ENGINE=MyISAM 
DEFAULT CHARSET=utf8mb4
COLLATE=utf8mb4_general_ci;

ALTER TABLE mydatabase.customers MODIFY COLUMN id bigint auto_increment NOT NULL;
```


for postgresql create table;
``` sql
CREATE TABLE customers (
  id        SERIAL PRIMARY KEY,
  name      VARCHAR(100) NOT NULL,
  email  	VARCHAR(100) NULL
);
```

for mongodb;
``` sql
db.createCollection("Customer");
```

## RUN
---------------------
``` bash
cp .env.example .env # end set your correct connection defination
```
Run with npm
``` bash
npm start
```
or docker compsoe
``` bash
docker compose up -d # docker port 3034
```
---------------------

## Success run looks like

![screenshot](./docs/success_run_main.png)

## CRUD Operation Success run looks like

![screenshot](./docs/list.png)

## Mongo ScreenShots
![screenshot](./docs/mongo_driver.png)

![screenshot](./docs/mongo_post.png)

![screenshot](./docs/mongo_list.png)

## Test
Before running the tests, make sure that the customers tables exist in the databases.

![screenshot](./docs/test_result.png)

