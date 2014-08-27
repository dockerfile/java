## Java Dockerfile


This repository contains **Dockerfile** of [Java](https://www.java.com/) for [Docker](https://www.docker.io/)'s [trusted build](https://index.docker.io/u/hseeberger/java/) published to the public [Docker Registry](https://index.docker.io/).


### Dependencies

* [dockerfile/ubuntu](http://dockerfile.github.io/#/ubuntu)


### Installation

1. Install [Docker](https://www.docker.io/).

2. Download [trusted build](https://index.docker.io/u/hseeberger/java/) from public [Docker Registry](https://index.docker.io/): `docker pull hseeberger/java`

   (alternatively, you can build an image from Dockerfile: `docker build -t="hseeberger/java" github.com/hseeberger/java`)


### Usage

    docker run -it --rm hseeberger/java

#### Run `java`

    docker run -it --rm hseeberger/java java

#### Run `javac`

    docker run -it --rm hseeberger/java javac
