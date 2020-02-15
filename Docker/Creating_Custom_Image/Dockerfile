# Using an existing docker image as our base
FROM alpine

# We then download and install a dependency
RUN apk add --update redis
RUN apk add --update gcc

# Tell the image what to do when it starts as a container i.e define the startup command
CMD ["redis-server"]

# Open the docker cmd line and navigate to the directory containing the dockerfile
# cd /F/Concor/......./Creating_Custom_Image
# docker build . 