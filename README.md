# zz-build-jpeg-recompress
[![build](https://github.com/iamasc8277/zz-build-jpeg-recompress/actions/workflows/build.yml/badge.svg)](https://github.com/iamasc8277/zz-build-jpeg-recompress/actions/workflows/build.yml) &ensp; [![release](https://github.com/iamasc8277/zz-build-jpeg-recompress/actions/workflows/release.yml/badge.svg)](https://github.com/iamasc8277/zz-build-jpeg-recompress/actions/workflows/release.yml)

binaries for jpeg-recompress 2.2.0 from [jpeg-archive](https://github.com/danielgtaylor/jpeg-archive):

download binary from [release 2.2.0](https://github.com/iamasc8277/zz-build-jpeg-recompress/releases/tag/v2.2.0)

or from docker image
* pull
  ```
  docker pull ghcr.io/iamasc8277/zz-build-jpeg-recompress:2.2.0
  ```
* or build locally
  ```
  docker build -t ghcr.io/iamasc8277/zz-build-jpeg-recompress:2.2.0 .
  ```
* and extract binary
  ```
  container_id=$(docker create ghcr.io/iamasc8277/zz-build-jpeg-recompress:2.2.0)
  docker cp "$container_id:/build/jpeg-archive/jpeg-recompress" jpeg-recompress
  docker rm "$container_id"
  ./jpeg-recompress --version
  ```
