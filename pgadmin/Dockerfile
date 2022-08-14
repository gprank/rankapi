FROM dpage/pgadmin4:latest

COPY ./config/docker_pgadmin_servers.json /pgadmin4/servers.json

ENTRYPOINT ["/bin/sh", "-c", "/bin/echo 'db:5432:*:ash:pokemon' > /tmp/pgpassfile && chmod 600 /tmp/pgpassfile && /entrypoint.sh"]
