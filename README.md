## Psalm - a static analysis tool for finding errors in PHP applications
[![Docker Pulls](https://img.shields.io/docker/pulls/rvannauker/psalm.svg)](https://hub.docker.com/r/rvannauker/psalm/) [![Docker Stars](https://img.shields.io/docker/stars/rvannauker/psalm.svg)](https://hub.docker.com/r/rvannauker/psalm/) [![](https://images.microbadger.com/badges/image/rvannauker/psalm:latest.svg)](https://microbadger.com/images/rvannauker/psalm:latest) [![GitHub issues](https://img.shields.io/github/issues/RichVRed/docker-psalm.svg)](https://github.com/RichVRed/docker-psalm) [![license](https://img.shields.io/github/license/RichVRed/docker-psalm.svg)](https://tldrlegal.com/license/mit-license)

Docker container to install and run psalm

### Installation / Usage
1. Install the rvannauker/psalm container:
```bash
docker pull rvannauker/psalm
```
2. Run psalm through the psalm container:
```bash
sudo docker run --rm --volume $(pwd):/workspace --name="psalm" "rvannauker/psalm" {destination}
```

### Download the source:
To run, test and develop the PSALM Dockerfile itself, you must use the source directly:
1. Download the source:
```bash
git clone https://github.com/RichVRed/docker-psalm.git
```
2. Build the container:
```bash
sudo docker build --force-rm --tag "rvannauker/psalm" --file psalm.dockerfile .
```
3. Test running the container:
```bash
 $ docker run rvannauker/psalm --help
```