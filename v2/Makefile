NACOS_VERSION ?= 2.0.3
TOOLS_SHELL="./hack/tools.sh"

prepare:
	docker pull nacos/nacos-server:$(NACOS_VERSION)
	docker run --rm --name nacos-quick -e MODE=standalone -p 8848:8848 -p 9848:9848 -d nacos/nacos-server:$(NACOS_VERSION)

stop:
	docker stop nacos-quick
