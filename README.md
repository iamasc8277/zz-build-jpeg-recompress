# zz-build-jpeg-recompress:2.2.0  &ensp; [![build](https://github.com/iamasc8277/zz-build-jpeg-recompress/actions/workflows/build.yml/badge.svg)](https://github.com/iamasc8277/zz-build-jpeg-recompress/actions/workflows/build.yml)

* download binary from [release 2.2.0](https://github.com/iamasc8277/zz-build-jpeg-recompress/releases/tag/v2.2.0)
* pull docker image
  ```
  docker pull ghcr.io/iamasc8277/zz-build-jpeg-recompress:2.2.0
  ```
* build docker image
  ```
  docker build -t ghcr.io/iamasc8277/zz-jpeg-recompress:2.2.0 .
  ```
* extract binary from docker image
  ```
  container_id=$(docker create ghcr.io/iamasc8277/zz-jpeg-recompress:2.2.0)
  docker cp "$container_id:/build/jpeg-archive/jpeg-recompress" jpeg-recompress
  docker rm "$container_id"
  ./jpeg-recompress --version
  ```
