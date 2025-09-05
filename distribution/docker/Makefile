all: build
image=registry.bizsaas.net/devops/nacos-server:2.5.1-jdk17
push:
	cp ../target/nacos-server-*.tar.gz ./;\
	docker buildx build --builder maven --pull --platform linux/amd64,linux/arm64 -t $(image) . --push
inspect:
	docker buildx imagetools inspect $(image)
