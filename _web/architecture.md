---
title: Website Architecture
layout: default
---


The LF website began as a highly-customized WordPress site. For obvious reasons we are moving away from this platform and moving toward a more service-oriented architecture. All micro services can be found in the [services repo](https://github.com/labfellows/services) and are prototyped in Python. Once a service becomes mission-critical, it may be rewritten into some other language built for long-running services (C++, Clojure, Scala, Haskell, etc) and moved into its own repo, while maintaining the same API.


## Services

The below services are in development. 

* **ERG** - connects the [typeform](http://helpcenter.typeform.com/hc/en-us/articles/200071986) data with the WordPress signup form over a REST interface.

## Reference

### Microservices

* [Martin Fowler on microservices](http://martinfowler.com/articles/microservices.html)
* [Microservices.io](http://microservices.io/patterns/microservices.html)

### Python Packages

Some useful Python packages for microservices ([source](https://speakerdeck.com/gnrfan/restful-microservices-with-python))

* requests
* uritemplate
* rfc3339
* Tornado
* hal-json
* halogen
* collection-json
* negotiator
* Flask-Restless
* tastypie
* djangorestframework
* https://github.com/bnrfan/django-restful

### API Keys

| Service | Docs link | Key |
|---------|-----------|-----|
| Typeform | [helpcenter.typeform.com](http://helpcenter.typeform.com/hc/en-us/articles/200071986) | `d71e1ebef5b2ee766ba8ccf31b7d1fbc01845db6` |





