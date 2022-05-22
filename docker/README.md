# SWAT+ on docker

The SWAT+ images have been built for linux:arm64 and linux:amd64, and pushed to
the [Docker hub](https://hub.docker.com/r/crazyzlj/swatplus/tags).

## Usage

```shell
docker pull crazyzlj/swatplus:apline-<VERSION_MAJOR>.<VERSION_MINOR>.<VERSION_PATCH>
docker run -it -v /path/to/your/swatplus-model-data:/swatplus_data swatplus<VERSION_MAJOR>.<VERSION_MINOR>.<VERSION_PATCH>.gfort.rel

# For example,
docker pull crazyzlj/swatplus:apline-60.5.4
docker run -it -v /Users/ljzhu/Documents/tmp/swatplusdata:/swatplus_data crazyzlj/swatplus:alpine-60.5.4 swatplus60.5.4.gfort.rel
```