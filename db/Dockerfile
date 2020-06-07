FROM postgres:latest

RUN mkdir -p /usr/local/scripts/
WORKDIR /usr/local/scripts/

COPY ./db_init.sh /usr/local/scripts/

RUN chmod +x db_init.sh

ENV POSTGRES_USER postgres
ENV POSTGRES_PASSWORD root
ENV POSTGRES_DB memes

ADD pg_hba.conf /etc/postgresql/9.5/main/
ADD postgresql.conf /etc/postgresql/9.5/main/

# CMD [ "/bin/bash", "/usr/local/scripts/db_init.sh", "start" ]
