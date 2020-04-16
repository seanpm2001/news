---
layout: post
author: Fabrizio Montesi
title: Jolie 1.9.0 released
tags:
- jolie
- microservices
- release
---

Jolie 1.9.0 has been released. Get it from [https://jolie-lang.org/downloads.html](https://jolie-lang.org/downloads.html).


## Jolie and REST

This release includes new tools to automatise some common practices in the development of Jolie REST services.

Jolier is a new tool to aid in the exposure of a Jolie API following the REST style ([doc](https://jolielang.gitbook.io/docs/language-tools-and-standard-library/rest/jolier)).

Also, Jolie now comes with two tools to integrate with [OpenAPI](https://swagger.io/specification/):

- `jolie2openapi` produces an OpenAPI definition from a Jolie interface ([doc](https://jolielang.gitbook.io/docs/language-tools-and-standard-library/rest/jolie2openapi));
- `openapi2jolie` produces a Jolie interface from an OpenAPI definition ([doc](https://jolielang.gitbook.io/docs/language-tools-and-standard-library/rest/openapi2jolie)).


## Tracing

In preparation for a debugger, the tracing system of the interpreter has been improved.

You can now also visualise the execution trace of a service using a [new jolietraceviewer tool](https://jolielang.gitbook.io/docs/language-tools-and-standard-library/tracing).


## Other changes

- The build system used to compile Jolie has been ported to Maven.
- Jolie is now compatible with Java 11 and beyond without requiring special configurations.
- Infinite alias loops are now detected at runtime and throw a fault.
- The `auto` self-configuring location now supports reading from JSON files ([doc](https://jolielang.gitbook.io/docs/language-tools-and-standard-library/locations#json-file)).
- Secure protocols (like HTTPS) now use TLSv1.2 by default.
- A lot of small fixes and code optimisations.