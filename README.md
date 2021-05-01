# 🦇 BatPonto App 🦇

### It's an app to register work time to employees from a Company.

## How to up PostgreSQL:

**Obs: You need to have Docker in your system.**
###### Download Docker [**Here**](https://www.docker.com/get-started).

Now we need to set up postgres database. We can get it from the Docker Hub. But we need to create a volume for store data.

`docker create -v /var/lib/postgresql/data --name PostgresData alpine`

then, we create the database.

`docker run -p 5432:5432 --name postgres -e POSTGRES_PASSWORD=minerva -d --volumes-from PostgresData postgres`
