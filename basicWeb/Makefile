all: build run
	echo "Build and run"
run:
	docker run --rm -it -p 8080:80 -v ./webContent/:/usr/share/nginx/html/ webdev_basic
build:
	docker build -t webdev_basic .