# Ursus

### Overview

Ursus is a [Dropwizard](http://dropwizard.codahale.com/) inspired framework for developing lightweight
production-ready web services on the JVM and [Grizzly](https://grizzly.java.net/). Ursus combines Grizzly's
NIO/Event Driven framework and popular libraries such as [Jersey 2.5](https://jersey.java.net/) and
[Project Tyrus - JSR 356: Java API for WebSocket - Reference Implementation](https://tyrus.java.net/) with
the simple found in Dropwizard, allowing you to focus on developing your services rather
than managing their accompanying dependencies, reducing time-to-market and maintenance.

#### Grizzly HTTP Container

Grizzly is a multi-protocol framework built on top of Java NIO. Grizzly aims to simplify development of
robust and scalable servers. Jersey provides a container extension module that enables support for using
Grizzly as a plain vanilla HTTP container that runs JAX-RS applications. Starting a Grizzly server to
run a JAX-RS or Jersey application is one of the most lightweight and easy ways how to expose a
functional RESTful services application.

#### REST / Jersey

Jersey is an open source, production quality, framework for developing RESTful Web Services in Java that
provides support for JAX-RS APIs and serves as a JAX-RS (JSR 311 & JSR 339) Reference Implementation.
Developing RESTful Web services with Jersey is a snap and the latest Jersey implementation included in
Ursus provides support for both asynchronous clients and server side services with [AsyncResponse](https://jax-rs-spec.java.net/nonav/2.0/apidocs/javax/ws/rs/container/AsyncResponse.html)

#### WebSockets / Tyrus

Tyrus is the open source [JSR 356](https://java.net/projects/websocket-spec) Java reference implementation of
WebSockets. The WebSocket protocol provides full-duplex communications between server and remote hosts.
WebSocket is designed to be implemented in web browsers and web servers, but it can be used by any client or server application.
The WebSocket protocol makes possible more interaction between a browser and a web site, facilitating live content
and the creation of real-time applications and services.

#### Additional Libraries

Ursus also includes many libraries found in Dropwizard and other frameworks and libraries to help speed up
development including,

* Logback and SLF4J bridging of Grizzly's java.util.logging
* Guava
* Hibernate Validator
* An Apache based HTTPClient and a Jersey 2.5 client
* Jackson for YAML and JSON parsing
* Joda time

