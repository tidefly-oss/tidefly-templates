# Tidefly Templates

> Community service deploy templates for [Tidefly](https://github.com/tidefly-oss/tidefly-plane) — self-hosted container management platform.

This repository contains ready-to-use deployment templates for common services. Templates are YAML files that Tidefly uses to deploy services with a single click.

## Repositories

| Repo                                                                  | Description                          |
|-----------------------------------------------------------------------|--------------------------------------|
| [tidefly-plane](https://github.com/tidefly-oss/tidefly-plane)         | Go API + deployment engine           |
| [tidefly-agent](https://github.com/tidefly-oss/tidefly-agent)         | Worker agent (gRPC mTLS)             |
| [tidefly-ui](https://github.com/tidefly-oss/tidefly-ui)               | SvelteKit frontend                   |
| [tidefly-tui](https://github.com/tidefly-oss/tidefly-tui)             | Bubble Tea setup wizard              |
| [tidefly-templates](https://github.com/tidefly-oss/tidefly-templates) | This repo — service deploy templates |
| [tidefly-docs](https://github.com/tidefly-oss/tidefly-docs)           | Documentation                        |

## Structure

```
tidefly-templates/
├── databases/        PostgreSQL, MySQL, Redis, MongoDB, ...
└── *.yaml            Docker Compose-based service templates
```

> Coming soon: `apps/`, `monitoring/`, `iam/`, and more.

## Contributing a Template

Community contributions are very welcome! See [CONTRIBUTING.md](CONTRIBUTING.md) for the template format and guidelines.

## License

[APGLv3](LICENSE)

---

<div align="center">
  <sub>Built with ❤️ by <a href="https://github.com/dbuettgen">@dbuettgen</a> · Part of the <a href="https://github.com/tidefly-oss">tidefly-oss</a> project</sub>
</div>