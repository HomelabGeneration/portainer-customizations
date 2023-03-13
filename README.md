# Portainer customizations

Holding portainer customizations like a custom list of application templates.

## Portainer startup command

By using the following startup options you can use the customizations provided by the repository.

```
docker run -d \
 -p 9443:9443 \
 --http-disabled \
 --name portainer \
 -v portainer_data:/data \
 -v /var/run/docker.sock:/var/run/docker.sock \
 --templates https://homelabgeneration.github.io/portainer-customizations/templates.json \
 --logo https://homelabgeneration.github.io/portainer-customizations/portainer_logo.png \
 portainer/portainer-ee:latest
```

