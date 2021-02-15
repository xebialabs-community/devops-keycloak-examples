FROM xebialabs/xl-release:10.0

# Install license
COPY conf/xl-release-license.lic /opt/xebialabs/xl-release-server/default-conf/

# Replace authentication plugin
RUN rm -f /opt/xebialabs/xl-release-server/default-plugins/xlr-official/xlr-auth-*.jar
COPY plugins /opt/xebialabs/xl-release-server/default-plugins

# Keycloak configuration
COPY conf/xl-release.conf /opt/xebialabs/xl-release-server/default-conf/reference.conf
