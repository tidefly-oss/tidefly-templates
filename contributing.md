# Contributing to Tidefly Templates

Community templates are the heart of this repo — contributions are very welcome!

## Template Format

Each template is a YAML file. Here's the basic structure:

```yaml
name: My Service
description: Short description of what this service does
version: "1.0"
icon: https://example.com/icon.png  # optional

env:
  - key: MY_PASSWORD
    description: Password for the service
    required: true
    secret: true
  - key: MY_PORT
    description: Port to expose
    default: "8080"

compose: |
  services:
    my-service:
      image: myimage:latest
      environment:
        PASSWORD: ${MY_PASSWORD}
      ports:
        - "${MY_PORT}:8080"
```

## Guidelines

- One template per file
- Use the official image from Docker Hub or GHCR where possible
- Always pin a specific image tag — never use `latest` in the `compose` block
- Mark sensitive values (passwords, tokens, keys) with `secret: true`
- Keep the template focused — one service per template
- Test your template locally with Tidefly before submitting

## Submitting a Template

1. Fork this repo
2. Add your template to the appropriate folder (or root if unsure)
3. Open a PR with a short description of what the service does

## Reporting Issues

Found a broken template? Open an issue with the template name and what went wrong.