# FIND.Base.Image

---

## How to build a base docker image for FIND

The resulting docker image should run on all platforms that are officially supported by docker. You can install [docker](https://docs.docker.com/engine/installation/) here

### Build the image

```
docker build \
    -t "skitol/findsar-base:latest" \
    -t "skitol/findsar-base:12.16.1" \
    .
```

### Push the tagged images to docker hub

```
docker push skitol/findsar-base:latest
docker push skitol/findsar-base:12.16.1
```

**Afterwards the image can be used via:**

```
docker run -it --rm skitol/findsar-base
```
