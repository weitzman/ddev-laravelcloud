[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/weitzman/ddev-laravelcloud/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/weitzman/ddev-laravelcloud/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/weitzman/ddev-laravelcloud)](https://github.com/weitzman/ddev-laravelcloud/commits)
[![release](https://img.shields.io/github/v/release/weitzman/ddev-laravelcloud)](https://github.com/weitzman/ddev-laravelcloud/releases/latest)

# DDEV Laravelcloud

## Overview

This add-on integrates Laravelcloud into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get weitzman/ddev-laravelcloud
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Laravelcloud |
| `ddev logs -s laravelcloud` | Check Laravelcloud logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.laravelcloud --laravelcloud-docker-image="ddev/ddev-utilities:latest"
ddev add-on get weitzman/ddev-laravelcloud
ddev restart
```

Make sure to commit the `.ddev/.env.laravelcloud` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `LARAVELCLOUD_DOCKER_IMAGE` | `--laravelcloud-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@weitzman](https://github.com/weitzman)**
