FROM alpine:latest

# Install CURL
RUN echo -e "https://mirror.tuna.tsinghua.edu.cn/alpine/v3.6/main\n\
https://mirror.tuna.tsinghua.edu.cn/alpine/v3.6/community" > /etc/apk/repositories

RUN apk --update add curl bash openjdk8 && \
      rm -rf /var/cache/apk/*

#install java
ADD jdk /usr/java/jdk

# Set environment
ENV JAVA_HOME /usr/lib/jvm/default-jvm
ENV PATH ${PATH}:${JAVA_HOME}/bin