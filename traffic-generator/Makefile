DOCKER_NAME ?= kiali/kiali-test-mesh-traffic-generator
DOCKER_TAG ?= latest

all: docker-build

docker-build:
	@echo Building the Kiali Test Mesh Traffic Generator Docker image
	@mkdir -p _output/docker
	@cp docker/* _output/docker
	@docker build -t ${DOCKER_NAME}:${DOCKER_TAG} _output/docker

clean:
	@echo "Cleaning any build artifacts"
	@echo "  - Removing the _output directory"
	@rm -rf _output
