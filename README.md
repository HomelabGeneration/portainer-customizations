# portainer-application-templates

Holding custom portainer application templates.

The application templates can be used in portainer by starting container like: 

```
docker run -d -p 9443:9443 --http-disabled --name portainer -v portainer_data:/data -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer-ee:latest --templates https://homelabgeneration.github.io/portainer-customizations/templates.json --logo https://homelabgeneration.github.io/portainer-customizations/portainer_logo.png
```

