all: build

build:
	cp ../target/nacos-server-1.4.0/nacos/target/nacos-server.jar  .;\
	docker build  -t registry.bizsaas.net/devops/nacos-server:1.4.0-security .

push:
	docker push registry.bizsaas.net/devops/nacos-server:1.4.0-security

.PHONY: all build push
