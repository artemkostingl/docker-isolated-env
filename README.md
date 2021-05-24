
***About:***
This is isolated environment for AOSP building.
It will be useful if you have to run any unsupported distribution and need to build Android OS.
This setup doesn't contain any repo managment tools in order to simplify setup and avoid credentials copying.
This environment is not as minimal as possible in order to cover as much as possible use cases.

**ATTENTION**
There is a W.A. for openjdk-8 that enables TLS1.0 and TLS1.1 as a quick fix.

1. Install Docker

Install Docker according to https://docs.docker.com/engine/install/

or

    **WARNING:** Always exam scripts that you are running

curl -fsSL https://get.docker.com | sh


1. Usage
```bash
make build
make run "<local_android_root_abs_path>"
make shell
```

2. Modification (only if needed)
    Edit Dockerfile and/or scripts and than use:
```bash
make build
make clean
make run "<local_android_root_abs_path>"
make shell
```
