FROM xebialabs/xl-deploy:23.3

# Keycloak configuration
COPY conf/*.yaml /opt/xebialabs/xl-deploy-server/centralConfiguration/
USER root
RUN chmod 777 /opt/xebialabs/xl-deploy-server/centralConfiguration/deploy-oidc.yaml
USER 1001