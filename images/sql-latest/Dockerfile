FROM mysql:latest

# Environment Variables
ENV MYSQL_ROOT_PASSWORD pwd123@
ENV MYSQL_DATABASE my_database
ENV MYSQL_USER dev
ENV MYSQL_PASSWORD pwd123

# Create user aubay
RUN useradd -ms /bin/bash aubay
USER aubay

# Copy the database schema to the /docker-entrypoint-initdb.d/ directory
COPY ./mysql/schema.sql /docker-entrypoint-initdb.d/

# Copy the database data to the /docker-entrypoint-initdb.d/ directory
COPY ./mysql/data.sql /docker-entrypoint-initdb.d/

# Expose port 3306
EXPOSE 3306
