VERSION=1.0
IMAGE_BASE=seldonio/mock_classifier

build_rest:
	s2i build -E environment_rest . seldonio/seldon-core-s2i-python2:0.2-SNAPSHOT ${IMAGE_BASE}_rest:${VERSION}

push_rest:
	docker push ${IMAGE_BASE}_rest:${VERSION}

build_grpc:
	s2i build -E environment_grpc . seldonio/seldon-core-s2i-python2:0.2-SNAPSHOT ${IMAGE_BASE}_grpc:${VERSION}

push_grpc:
	docker push ${IMAGE_BASE}_grpc:${VERSION}
