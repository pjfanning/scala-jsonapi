# Description

[![Build Status](https://travis-ci.org/kontainers/scala-jsonapi.svg)](https://travis-ci.org/kontainers/scala-jsonapi)
[![codecov.io](https://codecov.io/github/kontainers/scala-jsonapi/coverage.svg?branch=master)](https://codecov.io/github/kontainers/scala-jsonapi?branch=master)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/io.kontainers/scala-jsonapi_2.12/badge.svg)](https://maven-badges.herokuapp.com/maven-central/io.kontainers/scala-jsonapi_2.12)

scala-jsonapi is a Scala library that aims to help you produce JSON output based on the [JSON API specification][jsonapi] easily and painlessly. The library is compatible with Scala versions `2.11` and `2.12`. It supports read and write for the following backends:

 * [Play-JSON](https://www.playframework.com/documentation/2.6.x/ScalaJson)
 * [Spray-JSON](https://github.com/spray/spray-jsonn)


## Current Status

This library is very much a work in progress, so expect its API to change.

This is a fork of https://github.com/scala-jsonapi/scala-jsonapi, made with the intention of supporting play-json (and possibly some spray-json support) in Scala 2.11 and 2.12.

# Setup

To use scala-jsonapi, first add a library dependency — assuming that you have [sonatype resolvers] set up.

    libraryDependencies += "io.kontainers" %% "scala-jsonapi" % "0.7.0-SNAPSHOT"

You also have to provide the used backend (e.g. spray-json).

# Usage

The rich JSON API model is available via the following import:

    import org.zalando.jsonapi.model._

The library provides serialization and deserialization of JSON API root objects to JSON using Play-JSON (and Spray-JSON). Please note that you need to explicitly add a dependency for play-json (or spray-json) to your project.

# License

scala-jsonapi is licensed under the [MIT license](LICENSE) unless otherwise stated in the license files in higher directories (if any).

