# Web LLM docker service deployment
Set up guide for **Ollama** and **Open Webui** inside docker

## Set up docker
Install `docker.io` and `docker-compose-v2`   
Make sure the user is part of the docker group

## Install the NVIDIA Container Toolkit
Install NVDIA drivers to allow docker comtainers to access the low level GPU hardware   
https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html#prerequisites

## Containers set up
Get the files:
- run-compose.sh
- docker-compose.yaml
- docker-compose.gpu.yaml

from https://github.com/open-webui/open-webui/tree/main

## Containers execution
Start the services listening on port 80:   
`./run-compose.sh --enable-gpu --webui[port=80]`