This repository demonstrates a common mistake in Dockerfiles: using the `ubuntu:latest` base image. This image is large and can lead to inconsistent builds. The solution uses a slimmer and more specific image.

**Problem:**
The original `Dockerfile` uses `ubuntu:latest`, which is not a good practice due to its size and frequent updates, that could lead to unexpected breaking changes in the build process.

**Solution:**
The `Dockerfile-fixed` uses a smaller and more specific image like `ubuntu:22.04`, which will be consistent across builds unless explicitly changed.