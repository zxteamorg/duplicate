# Duplicate

[Manual](https://zxteamorg.github.io/duplicate/)

## Dev hints

### Build docs
```
rm -rf docs
docker build --tag docsbuilder --file docs.src/docker/Dockerfile docs.src
docker run --volume $(pwd):/development --entrypoint "mkdocs" docsbuilder build --clean --config-file ./docs.src/mkdocs.yml --site-dir ../docs/
touch docs/.nojekyll
```

### Block device from a regular file

1. Create a file
    ```
    dd if=/dev/random of=/tmp/my-file bs=1k count=1024
    ```
2. Associate loop devices with the file
    ```
    losetup -j /tmp/my-file
    ```
 