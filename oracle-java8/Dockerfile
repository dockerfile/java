#
# Oracle Java 8 Dockerfile
#
# https://github.com/dockerfile/java
# https://github.com/dockerfile/java/tree/master/oracle-java8
#

# Pull base image.
FROM ubuntu:17.04

# Install Java.
RUN \                                             
  echo oracle-java8-installer shared/accepted-oracle-license-v1-1 select true | debconf-set-selections \
  && apt-get update \
  && apt-get dist-upgrade \
  && DEBIAN_FRONTEND=noninteractive apt-get install -y apt-utils software-properties-common python-software-properties \
  && add-apt-repository ppa:webupd8team/java -y \
  && apt-get update \
  && DEBIAN_FRONTEND=noninteractive apt-get install -y oracle-java8-installer \
  && DEBIAN_FRONTEND=noninteractive apt-get install -y oracle-java8-set-default \
  && rm -rf /var/lib/apt/lists/* \
  && rm -rf /var/cache/oracle-jdk8-installer


# Define working directory.
WORKDIR /data

# Define commonly used JAVA_HOME variable
ENV JAVA_HOME /usr/lib/jvm/java-8-oracle
