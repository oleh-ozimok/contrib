all: push

# TAG 0.0 shouldn't clobber any release builds
TAG = 1.4
PREFIX = gcr.io/google_containers/echoserver

container:
	docker build --pull -t $(PREFIX):$(TAG) .

push: container
	gcloud docker push $(PREFIX):$(TAG)
