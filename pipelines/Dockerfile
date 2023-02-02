FROM mysql:latest

WORKDIR /scripts
COPY include/create_developer.template /scripts/

ENTRYPOINT ["docker-entrypoint.sh"]

EXPOSE 3306 33060

CMD ["mysqld"]
