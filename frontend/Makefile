APP_VERSION ?= 1.0
IMAGE_REGISTRY ?= us-central1-docker.pkg.dev/gowtham-demo-433405/frontend-reg
IMAGE_NAME ?= empms-frontend



install:
	npm install

build: install
	npm run build

image:
	docker build -t kaifshakeel/empms-frontend:1.0 -f Dockerfile .

push:
	docker push ${IMAGE_REGISTRY}/${IMAGE_NAME}:${APP_VERSION}
