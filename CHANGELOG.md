CHANGELOG
=========

3.5
---

 * Add `ServiceCollectionInterface`
 * Deprecate `ServiceSubscriberTrait`, use `ServiceMethodsSubscriberTrait` instead

3.4
---

 * Allow custom working directory in `TestHttpServer`

3.3
---

 * Add option `crypto_method` to `HttpClientInterface` to define the minimum TLS version to accept

3.2
---

 * Allow `ServiceSubscriberInterface::getSubscribedServices()` to return `SubscribedService[]`

3.0
---

 * Bump to PHP 8 minimum
 * Add native return types
 * Remove deprecated features

2.5
---

 *  Add `SubscribedService` attribute, deprecate current `ServiceSubscriberTrait` usage

2.4
---

 * Add `HttpClientInterface::withOptions()`
 * Add `TranslatorInterface::getLocale()`

2.3.0
-----

 * added `Translation\TranslatableInterface` to enable value-objects to be translated
 * made `Translation\TranslatorTrait::getLocale()` fallback to intl's `Locale::getDefault()` when available

2.2.0
-----

 * added `Service\Attribute\Required` attribute for PHP 8

2.1.3
-----

 * fixed compat with PHP 8

2.1.0
-----

 * added "symfony/deprecation-contracts"

2.0.1
-----

 * added `/json` endpoints to the test mock HTTP server

2.0.0
-----

 * bumped minimum PHP version to 7.2 and added explicit type hints
 * made "psr/event-dispatcher" a required dependency of "symfony/event-dispatcher-contracts"
 * made "symfony/http-client-contracts" not experimental anymore

1.1.9
-----

 * fixed compat with PHP 8

1.1.0
-----

 * added `HttpClient` namespace with contracts for implementing flexible HTTP clients
 * added `EventDispatcherInterface` and `Event` in namespace `EventDispatcher`
 * added `ServiceProviderInterface` in namespace `Service`

1.0.0
-----

 * added `Service\ResetInterface` to provide a way to reset an object to its initial state
 * added `Translation\TranslatorInterface` and `Translation\TranslatorTrait`
 * added `Cache` contract to extend PSR-6 with tag invalidation, callback-based computation and stampede protection
 * added `Service\ServiceSubscriberInterface` to declare the dependencies of a class that consumes a service locator
 * added `Service\ServiceSubscriberTrait` to implement `Service\ServiceSubscriberInterface` using methods' return types
 * added `Service\ServiceLocatorTrait` to help implement PSR-11 service locators
