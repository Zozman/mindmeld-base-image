# Mindmeld Base Image

Currently, [Mindmeld](https://github.com/cisco/mindmeld) does not provide a pre-built development image even though they do [publish a Dockerfile](https://github.com/cisco/mindmeld/blob/master/docker_containers/mindmeld_dep_docker/Dockerfile) for it.  Therefore this repo runs a GitHub Action every 24 hours to pull this Dockerfile, build it, and push it to the GitHub Container Registry so that there's a pre-built image that's up to date and usable to speed up builds.

## Tags

Images are tagged using the short and long SHA of the latest [Mindmeld master commit](https://github.com/cisco/mindmeld/commit/master) as of build time.  In addition the newest build is always tagged as `latest`.