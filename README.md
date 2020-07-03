# FIND.Base.Image
---

## Build docker image

```
    docker build \
        -t "skitol/findsar-base:latest" \
        -t "skitol/findsar-base:12.16.1" \
        .
```

## Push the tagged images to docker hub

```
    docker push skitol/findsar-base:latest
    docker push skitol/findsar-base:12.16.1
```

Afterwards the image can be used via:
```
    docker run -it --rm skitol/findsar-base
```