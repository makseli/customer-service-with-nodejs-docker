
# Customer Service with nodejs docker 

This is a customer service API Backend application. It is powered by NodeJS and Docker and allows you to use different databases (such as MongoDB, PostgreSQL, or MySQL). Thank you for your contributions.

TODO

- [x] Prepare development environment
- [x] Endpoint routing work with Express
- [x] MongoDB implementation
- [x] Posqresql implementation
- [x] Mysql implementation
- [ ] Write test :)
- [x] Run With Docker-Compose for development environment
- [ ] Run With Docker-Compose for production environment

for sql create table;
``` sql
CREATE TABLE mydatabase.customerss (
	id BIGINT NOT NULL,
	CONSTRAINT p_pk PRIMARY KEY (id),
	name varchar(100) NOT NULL,
	email varchar(100) NOT NULL
)
-- remove after for postgresql
ENGINE=MyISAM 
DEFAULT CHARSET=utf8mb4
COLLATE=utf8mb4_general_ci;
```

## Success run looks like

![screenshot](./docs/success_run_main.png)