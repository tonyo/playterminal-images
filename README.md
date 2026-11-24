# playterminal-images

Docker images for the PlayTerminal project. These images on DockerHub: https://hub.docker.com/u/playterminal/

Main project repo: https://github.com/rev112/playterminal/

The deployed instance: https://playtermin.al/

## Development

Needs [mise](https://mise.jdx.dev). In the repo root:

```sh
mise install && mise run setup   # pre-commit; installs the git hooks
mise run lint                    # ruff and the file checks on every file
```

The browser VM Image is built in [`v86/`](v86/README.md).
