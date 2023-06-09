all: build
image=registry.bizsaas.net/devops/nacos-server:2.2.3-SNAPSHOT
push:
	docker buildx build --pull --platform linux/amd64,linux/arm64 -t $(image) . --push
inspect:
	docker buildx imagetools inspect $(image)
