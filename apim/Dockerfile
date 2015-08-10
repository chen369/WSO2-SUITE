# rstuven/wso2-apim

FROM justinwalsh/centos-jre7

MAINTAINER Ricardo Stuven

ADD wso2am-1.9.0.zip /opt/

RUN unzip /opt/wso2am-1.9.0.zip -d /opt && \
    mv /opt/wso2am-1.9.0 /opt/wso2 && \
    rm /opt/wso2am-1.9.0.zip

WORKDIR /opt/wso2/

EXPOSE 9443
CMD ["/opt/wso2/bin/wso2server.sh"]
