TAG=latest
IMAGE=pg_tileserv

all: docker-build docker-push

docker-build-origin:
	docker build -f Dockerfile.alpine -t pramsey/pg_tileserv:latest-alpine .

docker-build:
	docker build -f pigeosolutions/Dockerfile.alpine.pigeo -t pigeosolutions/${IMAGE}:${TAG} ./pigeosolutions

docker-push:
	docker push pigeosolutions/${IMAGE}:${TAG}
