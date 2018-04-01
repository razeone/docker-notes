## Docker Images

Docker stores images in two places:

* Local store or local registry
* Docket Store (former Docker Hub) or public registry

First thing Docker does when you want to run an image is to verify that already exists in the local registry if it does, then execute it otherwise, proceedes to download it from the public registry.

So images are actually different from containers in the sense that are files and not a runtime, like a container it is.

We can explicitly pull images from public registry by executing:

```
docker image pull <name-of-the-image>
```

If we don't know the name of the image, we can search for it:

```
docker image search ubuntu
```

So now we can pull the ubuntu image and using the tag like this:

```
docker image pull ubuntu:17.04
```

That will give us a result list where the `ubuntu` keyword appears.

To get more information about images, we can search it in the [Docker Store](https://store.docker.com/) directly.

Another useful resource is to look for [docs in GitHub](https://github.com/docker-library/docs) for all official images.
