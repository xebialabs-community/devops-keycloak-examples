FROM xebialabs/xl-deploy:10.0

# Install license
COPY default-conf/deployit-license.lic /opt/xebialabs/xl-deploy-server/default-conf/

# Replace authentication plugin
RUN rm -f /opt/xebialabs/xl-deploy-server/lib/security-plugin-default-*.jar
COPY lib /opt/xebialabs/xl-deploy-server/lib

# Keycloak configuration
COPY default-conf/xl-deploy.conf /opt/xebialabs/xl-deploy-server/default-conf/reference.conf
