# Build image
docker build -t ubuntu .
# Run image
docker run -it --rm ubuntu -H
