# Pulp 3 Fedora 31 Container

This directory contains assets and tooling for building Pulp 3 container image based on Fedora 31.

For instructions how to run and use this container, see [Pulp in One Container](https://pulpproject.org/pulp-in-one-container/).

# Build instructions

```bash
$ wget https://github.com/just-containers/s6-overlay/releases/download/v1.22.1.0/s6-overlay-amd64.tar.gz
$ <docker build | buildah bud> --file pulp_ci/Containerfile --tag pulp/pulp-ci:latest .
$ <docker build | buildah bud> --file pulp_fedora31/Containerfile --tag pulp/pulp-fedora31:latest .
$ <docker build | buildah bud> --file pulp_galaxy_ng/Containerfile --tag pulp/pulp-galaxy-ng:latest .
```
