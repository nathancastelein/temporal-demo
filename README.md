![go workflow](https://github.com/garbage-collector/temporal-demo/actions/workflows/go.yml/badge.svg)

# temporal-demo

## Start Temporal

```bash
docker-compose up -d temporal-server temporal-ui
```

- server port: `7233`
- web port: `10000`

## Start the API

### Build the image

```bash
pack build myself --buildpack paketo-buildpacks/go --builder paketobuildpacks/builder-jammy-tiny
```

### Run the docker image

```bash
docker-compose up -d myself
```

- port: `8080`
