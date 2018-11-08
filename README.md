# MCJL - *Milagro Crypto Java Library*

[![Master Branch](https://img.shields.io/badge/-master:-gray.svg)](https://github.com/milagro-crypto/milagro-crypto-java/tree/master)
[![Master Build Status](https://secure.travis-ci.org/milagro-crypto/milagro-crypto-java.png?branch=master)](https://travis-ci.org/milagro-crypto/milagro-crypto-java?branch=master)
[![Master Coverage Status](https://coveralls.io/repos/github/milagro-crypto/milagro-crypto-java/badge.svg?branch=master)](https://coveralls.io/github/milagro-crypto/milagro-crypto-java?branch=master)

* **category**:    Library
* **copyright**:   2018 The Apache Software Foundation
* **license**:     ASL 2.0 ([Apache License Version 2.0, January 2004](http://www.apache.org/licenses/LICENSE-2.0))
* **link**:        https://github.com/milagro-crypto/milagro-crypto-java
* **introduction**: [AMCL.pdf](AMCL.pdf)


## Description

*MCJL - Milagro Crypto Java Library*

* MCJL is a standards compliant JavaScript cryptographic library with no external dependencies except for the random seed source.

* MCJL is a refactor of the *Java* code of [AMCL](https://github.com/milagro-crypto/amcl). For a detailed explanation about this library please read: [AMCL.pdf](AMCL.pdf). 

* MCJL supports the standards for RSA, ECDH, ECIES, ECDSA and M-PIN, AES-GCM encryption/decryption, SHA256, SHA384, SHA512 and SHA3 hash functions and a cryptographically secure random number generator. Furthermore we recently added New Hope, a post-quantum key exchange.

This library is created from the Java code in this directory 
[ACML](https://github.com/milagro-crypto/amcl/tree/master/version3/java) 
project. The config64.py script has been run in this AMCL directory and all 
the curves and RSA security level were selected for a 64-bit build; the output
Java files from this process are used in this project. If you require a 
smaller JAR file please follow the instructions in the AMCL project.

## Software Dependencies

In order to build this library, the following packages are required:

* [gradle](https://gradle.org/)

## Setup
This library is avaiable on Maven Central.

Replace `VERSION` below with required version.

To use `MCJL` with Maven project, use:
```
<dependency>
  <groupId>org.miracl.milagro.amcl</groupId>
  <artifactId>milagro-crypto-java</artifactId>
  <version>VERSION</version>
</dependency>
```

For Gradle project:
```
dependencies {
   compile 'org.miracl.milagro.amcl:milagro-crypto-java:VERSION'
}
```

Fill the `gradle.properties` file if you want to upload on Maven Central.

`MCJL` needs Java 8.

## Local Installation

Use this command to compile library and install it as artifact to local Maven 
repository.

    ./gradlew clean build publishToMavenLocal --stacktrace --info

## Contributions

Contributions are very welcome. Please make pull requests to the develop 
branch. You can run this command to build and test the code.

    ./gradlew build
