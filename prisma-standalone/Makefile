image_name = prisma-cli
build:
	docker build -t $(image_name) .

sh:
	# docker run --rm -it --platform linux/amd64 $(image_name) ash
	docker run --rm -it $(image_name) ash

run:
	docker run --rm $(image_name)
