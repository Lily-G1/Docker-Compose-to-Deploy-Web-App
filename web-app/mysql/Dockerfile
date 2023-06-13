FROM mysql:5.7
ENV MYSQL_DATABASE=db
ENV MYSQL_USER=user
ENV MYSQL_PASSWORD=password123
ENV MYSQL_ROOT_PASSWORD=password123
ADD . /tmp
RUN cp /tmp/db.sql /docker-entrypoint-initdb.d/db.sql
