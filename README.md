# fcrepo-karaf

Provides resources for provisioning Fedora Commons repository modules in [Karaf](http://karaf.apache.org).

[![Build Status](https://travis-ci.org/fcrepo4-labs/fcrepo-karaf.png?branch=master)](https://travis-ci.org/fcrepo4-labs/fcrepo-karaf)

[Fedora Commons Repository](https://github.com/fcrepo4/fcrepo4) modules are built as
OSGi bundles. This project makes it easy to provision these bundles in a Karaf-based
runtime. You will need at least version 4.x of Karaf to deploy Fedora modules.

## Installation

In order to install Fedora modules in Karaf, you must first add the `fcrepo-karaf`
feature repository. In the Karaf console:

    karaf> feature:repo-add mvn:org.fcrepo/fcrepo-karaf/LATEST/xml/features

To list the available `fcrepo` modules:

    karaf> feature:list | grep fcrepo

And to install individual `fcrepo` modules:

    karaf> feature:install fcrepo-http-api

## Maintainers

