FROM mysql:latest

COPY include/create_developer.sql /scripts/

RUN adduser jenkins sudo && \
    usermod -aG docker jenkins 
USER jenkins

ENTRYPOINT ["docker-entrypoint.sh"]

EXPOSE 3306 33060

CMD ["mysqld"]
