#
# OpenJDK Java 6 JRE Dockerfile
#
# https://github.com/dockerfile/java
# https://github.com/dockerfile/java/tree/master/openjdk-6-jre
#

# Pull base image.
FROM ubuntu:14.04

# Install Java.
RUN \
  apt-get update && \
  apt-get install -y openjdk-6-jre && \
  rm -rf /var/lib/apt/lists/*

# Define working directory.
WORKDIR /data

# Define commonly used JAVA_HOME variable
ENV JAVA_HOME /usr/lib/jvm/java-6-openjdk-amd64

# Define default command.
CMD ["bash"]
