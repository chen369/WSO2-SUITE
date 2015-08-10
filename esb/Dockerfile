# rstuven/wso2-esb

FROM justinwalsh/centos-jre7

MAINTAINER Ricardo Stuven

ADD wso2esb-4.8.1.zip /opt/

RUN unzip /opt/wso2esb-4.8.1.zip -d /opt && \
    mv /opt/wso2esb-4.8.1 /opt/wso2 && \
    rm /opt/wso2esb-4.8.1.zip

WORKDIR /opt/wso2/

EXPOSE 9443
CMD ["/opt/wso2/bin/wso2server.sh"]
