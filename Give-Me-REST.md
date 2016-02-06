# Give Me REST!!!

### Amanda Folson

## APIs (Application Programming Interfaces)

* Provides a uniform interface for interacting with your application

## Design

* Immutable blueprint

* SHARE

    * the worst feedback is the one you don't hear

* design for uniformity

* Contract between you and users

* **ASK! - **Build something people want

## Spec Tools

* API Blueprint 

* Swagger

## REST

* Representational State Transfer

* HTTP-based routing methods

* GET, POST, PUT, DELETE

HATEOAS

* Hypermedia As The Engine Of Application State

## When to Version

* When your API no longer meets you or your users' needs

* BUT NOT when you add new resources or data fields

## Version in URI

* https:/api.example.com/v1/resource

## Caching 

* Cache on client end

## Authentication

* Kill Basic Auth

    * Keep user/pass safe

* OAuth

    * requires users to explicitly authorize an app

    * tricky to implement

    * restrict to HTTPS endpoints

    * restricy domains allowed to auth

    * MITM attacks, make sure users store tokens well

## Security

* Treat users as hostile

* Dont rely on single method

* Apply layers of security

    * Permissions-based API keys/UAC

    * DNSBL

    * Content Type Length/depth limits

    * SQL Injection

    * Rate limit/throttling

## Prototyping

* larabel/lumen, flask, rails, mojolicious

    * RESTful HTTP routing

    * Zero to API in ~1h

* Specs

    * Apiary, Mockable, RAML

    * frameworks allow importing of specs

    * Some spec tools can autogenerate SDKs for your (APIMatic)

## Documentation

* API is useless if no one knows how to use it

* NEEDS to be part of design process

* All inclusive

    * Errors/methods/parameters

    * reference and tutorial

    * In sync with changes to API

* Include how to get help

* Open source is nice

## Resources

* http://apisyouwonthate.com

