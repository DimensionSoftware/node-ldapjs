# ldapjs Changelog

## CURRENT

- #201 Replace nopt with dashdash
- #134 Allow configuration of derefAliases client option
- #197 Properly dispatch unbind requests
- #196 Handle string ports properly in server.listen
- Request routing overhaul
    * #154 Route lookups do not depend on object property order
    * #111 Null ('') DN will act as catch-all
- Add basic server API tests
- Store EqualityFilter value as Buffer
- Run full test suite during 'make test'
- #190 Add error code 123 from RFC4370
- #178 Perform strict presence testing on attribute vals
- #183 Accept buffers or strings for cert/key in createServer
- #180 Add '-i, --insecure' option and to all ldapjs-\* CLIs

## 0.7.1

- #169 Update dependencies
    * asn1 to 0.2.1
    * pooling to 0.4.6
    * assert-plus to 0.1.5
    * bunyan to 0.22.1
- #173 Make dtrace-provider an optional dependency
- #142 Improve parser error handling
- #161 Properly handle close events on tls sockets
- #163 Remove buffertools dependency
- #162 Fix error event handling for pooled clients
- #159 Allow ext request message to have a buffer value
- #155 Make \*Filter.matches case insensitive for attrs

## 0.7.0

- #87 Minor update to ClientPool event pass-through
- #145 Update pooling to 0.4.5
- #144 Fix unhandled error during client connection
- Output ldapi:// URLs for UNIX domain sockets
- Support extensible matching of caseIgnore and caseIgnoreSubstrings
- Fix some ClientPool event handling
- Improve DN formatting flexibility
    * Add 'spaced' function to DN objects allowing toggle of inter-RDN when
      rendering to a string.  ('dc=test,dc=tld' vs 'dc=test, dc=tld')
    * Detect RDN spacing when parsing DN.
- #128 Fix user can't bind with inmemory example
- #139 Bump required tap version to 0.4.1
- Allow binding ldap server on an ephemeral port

## 0.6.3

- Update bunyan to 0.21.1
- Remove listeners on the right object (s/client/res/)
- Replace log4js with bunyan for binaries
- #127 socket is closed issue with pools
- #122 Allow changing TLS connection options in client
- #120 Fix a bug with formatting digits less than 16.
- #118 Fix "failed to instantiate provider" warnings in console on SmartOS

## 0.6.2 - 0.1.0

**See git history**
