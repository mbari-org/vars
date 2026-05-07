# Getting Started

VARS is deployed as a Docker-based stack managed by the [vars-quickstart-public](https://github.com/mbari-org/vars-quickstart-public) project. It provides the `varsq` CLI script that handles environment configuration, SSL certificate generation, and service lifecycle management.

## Prerequisites

- Docker Engine 20.10+ with Docker Compose V2
- Bash shell environment
- ~8 GB available RAM
- Network access to pull images from Docker Hub

## Setup Overview

The typical setup flow is:

1. Clone [vars-quickstart-public](https://github.com/mbari-org/vars-quickstart-public) and review available targets with `./varsq targets`
2. Configure your environment with `./varsq configure <target>`
3. Generate SSL certificates with `./varsq mkcert`
4. Start all services with `./varsq start`
5. Verify services are running with `./varsq status`

Full instructions, configuration reference, and troubleshooting guidance are in the [vars-quickstart-public repository](https://github.com/mbari-org/vars-quickstart-public).
