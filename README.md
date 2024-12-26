# Unreproducible Dockerfile
This Dockerfile demonstrates a common issue with using `ubuntu:latest` resulting in non-reproducible builds.  The fix uses a specific Ubuntu version tag.

**Bug:** The use of `ubuntu:latest` means the build depends on whatever the latest version of Ubuntu is at build time. This can change unexpectedly, causing build failures.

**Solution:** Use a specific version, such as `ubuntu:22.04`, to ensure reproducibility.