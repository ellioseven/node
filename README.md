# Node

A bundled `node` and `npm` executable.

## Usage

``` bash
docker run --rm -ti ellioseven/node:8 bash
```

## Tags

- `node:9`
- `node:8`
- `node:6`
- `node:4`

## Quick Notes

1. App directory is located in `/srv`
2. App directory node module binaries are added the `node` user path, `/srv/node_modules/.bin`
3. Global packages can be mounted to `/home/node/.npm-packages`
4. Global package binaries are added the the `node` user path, `/home/node/.npm-packages/bin`
5. Directly extends the [node](https://hub.docker.com/_/node/) images, so
  `yarn` is packaged for free.

Built with [Docker image templating system](https://github.com/ellioseven/docker-image-templating-system).
