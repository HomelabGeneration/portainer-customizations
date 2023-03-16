# Portainer customizations

Holding portainer customizations like a custom list of application templates.

## Portainer startup command

By using the following startup options you can use the customizations provided by the repository.

```
docker run -d \
 --name portainer \
 -p 9443:9443 \
 -v portainer_data:/data \
 -v /var/run/docker.sock:/var/run/docker.sock \
 --restart=always \
 portainer/portainer-ee:latest \
 --http-disabled \
 --templates https://homelabgeneration.github.io/portainer-customizations/templates.json \
 --logo https://homelabgeneration.github.io/portainer-customizations/portainer_logo.png
```

