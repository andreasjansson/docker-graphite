Graphite
========

Graphite server with optional HTTP auth. Also runs an SSH server on port 22 with username=`root`, password=`root`.

Loosely based on https://index.docker.io/u/nickstenning/graphite/

Environment variables
---------------------

* `HTTP_AUTH_USER`
  - If defined, will require the user to authenticate using this username
  - Optional, default undefined
* `HTTP_AUTH_USER`
  - If defined, will require the user to authenticate using this password
  - Optional, default undefined

Ports
-----

* 22
  - sshd
* 80
  - nginx graphite web gui
* 2003
  - carbon line receiver port
* 2004
  - carbon pickle receiver port
* 7002
  - carbon cache query port
