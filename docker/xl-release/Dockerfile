# Offical
FROM xebialabs/xl-release:10.0

# Install license
COPY default-conf/xl-release-license.lic /opt/xebialabs/xl-release-server/default-conf/

# Replace authentication plugin
RUN rm -f /opt/xebialabs/xl-release-server/default-plugins/xlr-official/xlr-auth-*.jar
COPY default-plugins /opt/xebialabs/xl-release-server/default-plugins

# Keycloak configuration
COPY default-conf/reference.conf /opt/xebialabs/xl-release-server/default-conf/
