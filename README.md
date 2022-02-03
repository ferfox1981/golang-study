# To create the image
docker build . -t alpine-golang

# To load the container
docker run --name alpine-golang-container -it -d alpine-golang

# To add bash
docker exec -it alpine-golang-container apk add bash

# To enter command
docker exec -it alpine-golang-container bash