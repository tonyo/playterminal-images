# playterminal-images

The VM Image for PlayTerminal: an i386 Alpine Linux image holding the Games, which the
site runs in the visitor's browser with the [v86](https://github.com/copy/v86) emulator.
How to build it and what it outputs: [`v86/README.md`](v86/README.md).

Main project repo: https://github.com/tonyo/playterminal

The deployed instance: https://playtermin.al/

Until the switch to v86, each Game ran on the server in its own Docker container, built
from this repo and published as `playterminal/*` on Docker Hub. Those Dockerfiles were
removed after commit cc93c51.

## Development

Needs [mise](https://mise.jdx.dev). In the repo root:

```sh
mise install && mise run setup   # pre-commit; installs the git hooks
mise run lint                    # ruff and the file checks on every file
```
