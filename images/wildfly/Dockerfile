FROM jboss/wildfly:14.0.1.Final

MAINTAINER Olivier Liechti <olivier.liechti@heig-vd.ch>

ADD LandingPageApp-1.0-SNAPSHOT.war /opt/jboss/wildfly/standalone/deployments/

ADD LandingPageMVCApp-1.0-SNAPSHOT.war /opt/jboss/wildfly/standalone/deployments/

RUN /opt/jboss/wildfly/bin/add-user.sh admin admin --silent

CMD ["/opt/jboss/wildfly/bin/standalone.sh", "-b", "0.0.0.0", "-bmanagement", "0.0.0.0"]

