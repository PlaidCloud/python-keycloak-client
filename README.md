# Python Keycloak Client

[![Build Status](https://www.travis-ci.org/Peter-Slump/python-keycloak-client.svg?branch=master)](https://www.travis-ci.org/Peter-Slump/python-keycloak-client)

Python Client for Keycloak identity and access management service

[Documentation](Python Client for Keycloak identity and access management service)

http://www.keycloak.org/
https://github.com/Peter-Slump/python-keycloak-client

## Development

Install development environment:

```bash
$ make install-python
```

### Writing docs

Documentation is written using Sphinx and maintained in the docs folder.

To make it easy to write docs Docker support is available.

First build the Docker container:

    $ docker build . -f DockerfileDocs -t python-keycloak-client-docs

Run the container

    $ docker run -v `pwd`:/src --rm -t -i -p 8050:8050 python-keycloak-client-docs

Go in the browser to http://localhost:8050 and view the documentation which get
refreshed and updated on every update in the documentation source.