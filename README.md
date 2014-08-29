## Java Dockerfile


This repository contains **Dockerfile** of [Java](https://www.java.com/) for [Docker](https://www.docker.io/)'s [trusted build](https://index.docker.io/u/dockerfile/java/) published to the public [Docker Registry](https://index.docker.io/).


### Dependencies

* [dockerfile/ubuntu](http://dockerfile.github.io/#/ubuntu)


### Installation

1. Install [Docker](https://www.docker.io/).

2. Download [trusted build](https://index.docker.io/u/dockerfile/java/) from public [Docker Registry](https://index.docker.io/): `docker pull dockerfile/java`

   (alternatively, you can build an image from Dockerfile: `docker build -t="dockerfile/java" github.com/dockerfile/java`)


### Docker Tags

`dockerfile/java` provides multiple tagged images:

* `latest` (default): alias to `openjdk-7-jre` (OpenJDK Java 7 JRE)
* `openjdk-6-jdk`: OpenJDK Java 6 JDK
* `openjdk-6-jre`: OpenJDK Java 6 JRE
* `openjdk-7-jdk`: OpenJDK Java 7 JDK
* `openjdk-7-jre`: OpenJDK Java 7 JRE
* `oracle-java6`: Oracle Java 6 JDK
* `oracle-java7`: Oracle Java 7 JDK
* `oracle-java8`: Oracle Java 8 JDK


### Usage

    docker run -it --rm dockerfile/java

#### Run `java`

    docker run -it --rm dockerfile/java java

#### Run `javac`

    docker run -it --rm dockerfile/java javac
