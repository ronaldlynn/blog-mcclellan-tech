---
layout: post
title:  "Get a Docker Container IP Address from the Host"
date:   2020-07-04 14:02:18 -0400
categories: docker
---
### Newer Docker:
`docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' container_name_or_id`

### Older Docker
`docker inspect --format '{{ .NetworkSettings.IPAddress }}' container_name_or_id`

### More information:
https://stackoverflow.com/questions/17157721/how-to-get-a-docker-containers-ip-address-from-the-host