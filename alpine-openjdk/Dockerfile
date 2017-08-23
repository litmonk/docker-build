FROM alpine:latest

# add repositories
RUN echo -e "https://mirror.tuna.tsinghua.edu.cn/alpine/v3.6/main\n\
https://mirror.tuna.tsinghua.edu.cn/alpine/v3.6/community" > /etc/apk/repositories

#install curl bash openjdk8
RUN apk --update add curl bash openjdk8 && \
      rm -rf /var/cache/apk/*

# Set environment
ENV JAVA_HOME /usr/lib/jvm/default-jvm
ENV PATH ${PATH}:${JAVA_HOME}/bin
