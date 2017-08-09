## Java Dockerfile

### Installation

1. Install [Docker](https://www.docker.com/).

### Usage
    cd oracle-java8
    docker build -t uandrew1965/java-sdk:1.8.0.144-b01 . ##(1.8.0_144-b01 version java-sdk now)
    docker run -it --name java-sdk-1.8.0.144-b01 uandrew1965/java-sdk:1.8.0.144-b01
    java -version


### Usage

    docker run -it --rm dockerfile/java

#### Run `java`

    docker run -it --rm dockerfile/java java

#### Run `javac`

    docker run -it --rm dockerfile/java javac
