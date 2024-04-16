all: build run
	echo "Build and run"
run:
	docker run --rm -it -p 8888:8888 -v "$(shell pwd)"/notebook:/notebook jupyter-mokulanis jupyter notebook --ip=0.0.0.0 --port=8888 --no-browser --allow-root
build:
	docker build -t jupyter-mokulanis .