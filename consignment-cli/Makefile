build:
	GOOS=linux GOARCH=386 go build .
	docker build -t consignment-cli .
	make build-clean
build-clean:
	rm consignment-cli
run:
	docker run -e MICRO_REGISTRY=mdns consignment-cli