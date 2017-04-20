IMAGE 		:= gcr.io/soon-fm-production/nginx
TAG 		:= latest

image:
	docker build -f Dockerfile --force-rm -t $(IMAGE):$(TAG) .
	gcloud docker -- push $(IMAGE):$(TAG)
