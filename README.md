## Java Dockerfile


This repository contains **Dockerfile** of [Java](https://www.java.com/) for [Docker](https://www.docker.com/)'s [automated build](https://registry.hub.docker.com/u/dockerfile/java/) published to the public [Docker Hub Registry](https://registry.hub.docker.com/).


### Base Docker Image

* [dockerfile/ubuntu](http://dockerfile.github.io/#/ubuntu)


### Docker Tags

`dockerfile/java` provides multiple tagged images:

* `latest` (default): OpenJDK Java 7 JRE (alias to `openjdk-7-jre`)
* `openjdk-6-jdk`: OpenJDK Java 6 JDK
* `openjdk-6-jre`: OpenJDK Java 6 JRE
* `openjdk-7-jdk`: OpenJDK Java 7 JDK
* `openjdk-7-jre`: OpenJDK Java 7 JRE
* `oracle-java6`: Oracle Java 6 JDK
* `oracle-java7`: Oracle Java 7 JDK
* `oracle-java8`: Oracle Java 8 JDK

For example, you can run a `Oracle Java 8` container with the following command:

    docker run -it --rm dockerfile/java:oracle-java8 java -version


### Installation Guide

1. Install [Docker](https://www.docker.com/).

2. Download [automated build](https://registry.hub.docker.com/u/dockerfile/java/) from public [Docker Hub Registry](https://registry.hub.docker.com/): `docker pull dockerfile/java`

   (alternatively, you can build an image from Dockerfile: `docker build -t="dockerfile/java" github.com/dockerfile/java`)


### Usage

    docker run -it --rm dockerfile/java

#### Run `java`

    docker run -it --rm dockerfile/java java

#### Run `javac`

    docker run -it --rm dockerfile/java javac
