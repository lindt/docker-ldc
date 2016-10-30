[![Docker pulls](https://img.shields.io/docker/pulls/dlanguage/ldc.svg)](https://hub.docker.com/r/dlanguage/ldc/)
[![Docker Build](https://img.shields.io/docker/automated/dlanguage/ldc.svg)](https://hub.docker.com/r/dlanguage/ldc/)

# docker-LDC

Docker Image for LDC

## Usage

Place a `test.d` in your current directory.
Then execute
```
docker run --rm -ti \
  -e USER -e HOME -e LOCAL_USER_ID=`id -u $USER` -e LOCAL_GROUP_ID=`id -g $USER`
  -w $(pwd) \
  -v /home/$USER:/home/$USER \
  dlanguage/ldc ldc2 test.d
```
