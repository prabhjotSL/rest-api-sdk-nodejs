PayPal Node SDK release notes
============================

v1.0.1
----
* Update Paypal-Client-Metadata-Id header for future payments
* Subscription API changes for searching transactions and listing billing plans

v1.0.0
----
### Features
* Subscription API support added
* Order/Auth/Capture support added
* Update credit card support added for vault
* Test/samples added for extra payment parameters
* activate method added for billing plans

### Breaking changes
* Exported methods are now camelCased instead of underscored in 0.* versions
* delete is now del
* support still maintained for above changes for compatibility with 0.* versions

### Refactoring
* Modularize into components api, client, config and utils
* Rest api resources separated into own functions/classes
* generate has the factory of rest methods attached to object literals e.g creditCard, reducing duplication
* Exported methods named and CamelCased across sdk, closer to JavaScript conventions, closes #34 and #35
* Test coverage increased

v0.9.1
----
* Fix for toggling host by using mode in config

v0.9.0
----
* Unit tests can run as mock mode
* Mode configuration for easier toggling between live/sandbox
* NODE_ENV=development can be added for getting debug-id

v0.8.0
-----
* Invoicing API support added 
* Added tests and samples for using the invoicing api via the sdk
* Modules pinned to versions for package.json

v0.7.0
-----
* Future Payments support added
* Linting

v0.6.4
-----
* Fixed content length to support utf-8 characters

v0.6.3
-----
* Added support for Reauthorization.

v0.6.2
-----
* Update HTTP User-Agent

v0.6.1
-----
* Allow payment.list with parameters
