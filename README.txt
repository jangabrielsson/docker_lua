docker buildx create --name pibuilder
docker buildx use pibuilder
docker buildx inspect --bootstrap
docker buildx build --platform linux/arm/v7 -t jangabrielsson/lua5.3:latest --push .
