# Use an existing docker image as a base
FROM alpine

# Adding alpine repositories to fix the alert of ssl certifcate issue behind proxy
COPY repositories /etc/apk/repositories

# Download and install a dependency
RUN apk add --update redis
RUN apk add --update gcc

# Tell the image what to do when it starts as a container
CMD ["redis-server"]
