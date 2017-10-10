# Build with GNU Make

[![CircleCI](https://circleci.com/gh/Praqma/native-example-make.png?style=shield&circle-token=df3dc5f6efbc2a267f7805f05a5e91d2878be9fd)](https://circleci.com/gh/Praqma/native-example-make)
[![TravisCI Status](https://travis-ci.org/Praqma/native-example-make.svg?branch=master)](https://travis-ci.org/Praqma/native-example-make)

![](https://img.shields.io/github/stars/praqma/native-example-make.svg)
![](https://img.shields.io/github/forks/praqma/native-example-make.svg)
![](https://img.shields.io/github/watchers/praqma/native-example-make.svg)
![](https://img.shields.io/github/tag/praqma/native-example-make.svg)
![](https://img.shields.io/github/release/praqma/native-example-make.svg)
![](https://img.shields.io/github/issues/praqma/native-example-make.svg)

Building with [GNU Make](https://www.gnu.org/software/make/) inside [container](https://hub.docker.com/r/praqma/native-make/).

See [native](https://github.com/Praqma/native) repository for more examples.

## Exercise 1 - Create your own fork of this project

Make your own fork of this project for you to develop on.

## Exercise 2 - Build and test your project on the jenkins servier

    make clean
    make all
    make test

## Exercise 3 - Test results

Add a `Post Build Action` to your job to publish the junit test result.

## Exercise 4 - Publish Artifacts

Add a `Post Build Action` to your job to publish the binary.
## Steps

* Run container: `./docker-run.sh`
* Build example (inside container): `make all`
* Test example (inside container): `make test`
