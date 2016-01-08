FROM tutum/jboss:as7
MAINTAINER Rafael Gomes <rgomes@thoughtworks.com>

COPY standalone.xml /jboss-as-7.1.1.Final/standalone/configuration/standalone.xml

COPY run.sh /run.sh
RUN chmod +x /*.sh
RUN mkdir -p /jboss-as-7.1.1.Final/modules/org/postgresql/main

COPY module.xml /jboss-as-7.1.1.Final/modules/org/postgresql/main/module.xml

EXPOSE 8080 9990
CMD ["/run.sh"]
