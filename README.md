## dotproxy
**dotproxy** is an app written in Python that implements DNS-over-TLS on TCP.
It does so by receiving standard DNS requests, wrapping them on an SSL-wrapped socket and resolving using 1.1.1.1 DNS resolver over TLS on port 853.

## Run
Install python 3.7 and run:

    python3 server.py

## Test
    Windows:
    nslookup "-set vc" example.com 127.0.0.1

	Linux:
	dig example.com @127.0.0.1 +tcp
