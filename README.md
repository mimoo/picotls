picotls
===

Picotls is a TLS 1.3 implementation written in C.

The primary goal of the project is to create a tiny but fast TLS 1.3 implementation that can be used with the HTTP/2 protocol stack and the upcoming QUIC stack of the [H2O HTTP/2 server](https://h2o.examp1e.net).

How to
---

Build using cmake:
```
% cmake
% make
```

Run the test server (at 127.0.0.1:8443):
```
% ./cli -c /path/to/certificate.pem -k /path/to/private-key.pem  127.0.0.1 8443
```

Connect to the test server:
```
% ./cli 127.0.0.1 8443
```