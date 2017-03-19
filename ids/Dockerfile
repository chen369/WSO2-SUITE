# rstuven/wso2-ids

FROM chen369/WSO2-SUITE:centos

MAINTAINER Chen Chiu
ARG IS_VERSION=${VERSION:-5.3.0}
RUN wget -P /opt https://s3-us-west-2.amazonaws.com/wso2-stratos/wso2is-${IS_VERSION}.zip && \
    unzip /opt/wso2is-${IS_VERSION}.zip -d /opt && \
    mv /opt/wso2is-${IS_VERSION} /opt/wso2 && \
    rm /opt/wso2is-${IS_VERSION}.zip

WORKDIR /opt/wso2/

EXPOSE 9443
CMD ["/opt/wso2/bin/wso2server.sh"]
