# Docker Commands

## Pull an Image 
`
docker pull <image_name>
`
## Start an Image with a given Alias
`
docker run --name <container_alias> <image_name>
`

If you don't specify an alias, I random one will be used

## Start an Image with a Port Mapping
`
docker run -p <port_host>:<port_container> <image_name>
`

## Start an Image in the Background
`
docker run -d <image_name>
`

---

## Trail logs of the container
`
docker logs -f <container_alias>
`
## List the running containers
`
docker ps
`
## Stop a container
`
docker stop <container_alias>
`
## Open Shell inside a container
`
docker exec -it <container_alias> sh
`
## List all local Images with Image size
`
docker images
`

