FROM jboss/wildfly

#ADD customization/Netgifx.war /opt/jboss/wildfly/standalone/deployments/


ADD customization /opt/jboss/wildfly/customization/
RUN cat "/opt/jboss/wildfly/customization/execute.sh"

RUN ls -lha "/opt/jboss/wildfly/customization/execute.sh"

CMD ["/opt/jboss/wildfly/customization/execute.sh"]


#RUN /opt/jboss/wildfly/bin/add-user.sh admin Admin#70365 --silent

#CMD ["/opt/jboss/wildfly/bin/standalone.sh", "-b", "0.0.0.0", "-bmanagement", "0.0.0.0"]