# Challenge Instructions

This challenge consists of three containers: Nginx, MySQL and NodeJS. When a user accesses Nginx, a request should be made to the NodeJS app that'll then add an entry to a MySQL database.

## COS:

1. `docker-compose up -d` should be the only command necessary to spin all up;
2. http://localhost:8080 should return `<h1>Full Cycle Rocks!</h1>` plus the names in the DB;
3. MySQL should retain its data in a local volume.
