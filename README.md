# Basalt Unraid Template

Unraid Docker template and automated build for [Basalt](https://github.com/jesdga95/basalt) — a local LLM inference engine for NVIDIA Blackwell GPUs.

## Requirements

- NVIDIA Blackwell GPU (RTX 5090/5080, B200, GB200)
- NVIDIA driver R580+
- NVIDIA Container Runtime configured in Unraid

## Setup

1. Add this template repository URL to Unraid: `https://github.com/jbowensii/basalt-unraid`
2. Install the **basalt** template from Community Applications
3. Copy `basalt_config.json` to `/mnt/user/appdata/basalt/basalt_config.json`
4. Download models with `docker exec basalt basalt download <model-name>`

## Image

Built weekly from upstream via GitHub Actions → `ghcr.io/jbowensii/basalt:latest`.

Trigger a manual build from the Actions tab anytime.
