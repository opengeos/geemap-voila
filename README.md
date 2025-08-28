---
title: Geemap Voila
emoji: 🚀
colorFrom: red
colorTo: red
sdk: docker
app_port: 7860
tags:
  - geemap
pinned: false
short_description: A Voila template for geemap
license: mit
---

# geemap-voila

Build a docker image for using geemap with Voila

To build the image:

```bash
docker buildx build --platform linux/amd64,linux/arm64 -t giswqs/geemap:voila --push .
```

To run the image:

```bash
docker run -it -p 7860:7860 -v $(pwd):/home/jovyan/notebooks giswqs/geemap:voila
```

To push the image to the registry:

```bash
docker push giswqs/geemap:voila
```
