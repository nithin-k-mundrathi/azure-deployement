
# docker Host address
http://localhost:8080/

# Build the docker Image
docker build . -f Dockerfile.streamlit -t azuredeploy

# Run the docker 
docker-compose up

# docker login  to azure created Container registry
docker login mentalhealthstreamlit.azurecr.io

# push ur current Image
docker push <ImageName> ImageName should match the Azuere Container Registry Webregistry

