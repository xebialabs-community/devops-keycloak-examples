FROM jboss/keycloak

ARG KEYCLOAK_USER
ARG KEYCLOAK_PASSWORD

ADD . /tmp/source

ENV KEYCLOAK_USER=${KEYCLOAK_USER:-admin} KEYCLOAK_PASSWORD=${KEYCLOAK_PASSWORD:-admin}

CMD ["-b", "0.0.0.0", \
     "-Dkeycloak.migration.action=import", \
     "-Dkeycloak.migration.provider=dir", \
     "-Dkeycloak.migration.dir=/tmp/source/realm-xlr", \
     "-Dkeycloak.migration.realmName='digitalai-platform'"]
