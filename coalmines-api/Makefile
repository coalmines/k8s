APP_DIR := app
APP_TAG := coalmines-api

all: build docker-image

build:
	@$(MAKE) -C $(APP_DIR)

docker-image:
	eval $(minikube docker-env) && \
		docker build -t $(APP_TAG) .
