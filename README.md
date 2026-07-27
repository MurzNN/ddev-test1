[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/MurzNN/ddev-test1/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/MurzNN/ddev-test1/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/MurzNN/ddev-test1)](https://github.com/MurzNN/ddev-test1/commits)
[![release](https://img.shields.io/github/v/release/MurzNN/ddev-test1)](https://github.com/MurzNN/ddev-test1/releases/latest)

# DDEV Test1

## Overview

This add-on integrates Test1 into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get MurzNN/ddev-test1
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Test1 |
| `ddev logs -s test1` | Check Test1 logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.test1 --test1-docker-image="ddev/ddev-utilities:latest"
ddev add-on get MurzNN/ddev-test1
ddev restart
```

Make sure to commit the `.ddev/.env.test1` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `TEST1_DOCKER_IMAGE` | `--test1-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@MurzNN](https://github.com/MurzNN)**
