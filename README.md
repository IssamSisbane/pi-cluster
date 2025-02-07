# PI Cluster
A GitOps Repository for a K3S cluster running on a Raspberry PI.

I began learning about GitOps through Mischa van den Burg's Homelab course in the Kubecraft community.

This repository showcases everything I have learned from the course.

## What is running ?

Inside this cluster we have for now only one application running called Linkding.
[Linkding](https://github.com/sissbruecker/linkding)  is a selfhost bookmark manager.

It's really easy to setup and so it's create to use as an application for my experimentations.

## TOOLS

- K3S : Kubernetes Distribution
- Cloudflare Tunnels (cloudflared) : To expose our homelab to Internet
- SOPS : To managing safely secrets

## TODO

- [ ] Add devcontainer config
- [X] Add Persistent storage to Linkding
- [X] Make sure the container runs as non root & disable privilege escalation
- [X] Expose Linkding to Internet
  - [X] Setup a Cloudflare Tunnels & a linkding service
  - [ ] Configure Traefik Ingress
- [X] Add SOPS to protect secret
- [ ] Add SSL Certificates to allow https
