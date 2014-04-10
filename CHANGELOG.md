# Chef Push Client Changelog

## 1.0.2 (2014-04-10)

### Chef Push Client 1.0.1

* Add require with rescue for chef/config_fetcher needed for compatibility with
  Chef >= 11.8.0.

* Add signal handling for the client. The client now does a graceful
  shutdown when it receives a `TERM`, `QUIT`, or `KILL` signal. The
  client will reconfigure itself if sent `USR1`. This improves the
  compatibility of the push client to be managed under runit which
  sends signals for restart.

### chef
* upgrade to version 11.10.4

### libyaml 0.1.6

* CVE-2014-2525: Heap-based buffer overflow allows context-dependent
  attackers to execute arbitrary code

### openssl 1.0.1g

* CVE-2014-0160: heartbeat extension allows remote attackers to obtain
  sensitive information from process memory


## 1.0.1

pre-changelog Chef Push Client
