FROM amd64/debian:10-slim
MAINTAINER snxx

WORKDIR /toit
ENV TOIT_HOME=/toit
ENV TOIT_VERSION 0.11.1

ADD https://github.com/toitlang/toit/releases/download/v$TOIT_VERSION/toit-linux.tar.gz .
RUN gunzip ./toit* && mv ./toit* /bin/toit && chmod +x /bin/toit

LABEL version="/$TOIT_VERSION"
LABEL description="Toit - IoT software platform for the ESP32"
LABEL maintainer="snxx.lppxx@gmail.com"

CMD "/bin/toit"
