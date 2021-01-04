# code-server

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![](https://img.shields.io/static/v1?label=Platforms&message=linux/amd64,linux/arm64&color=orange)
![](https://img.shields.io/static/v1?label=Python&message=3.6&color=red)
![](https://img.shields.io/static/v1?label=build&message=passing&color=green)



*** CopyRight 2020 Kevin Yu. All rights reserved.

*** Author: Kevin Yu

*** Update Time: 2021/01/02

Run [VS Code](https://github.com/Microsoft/vscode) on any machine anywhere and access it in the browser

![](https://github.com/yqlbu/code-server/blob/main/demo.png?raw=true)

## Highlights

- Code on any device with a consistent development environment
- Use remote servers either Public or Private Cloud to speed up tests, compilations, downloads, and more
- Continue the development workflow remotely and get work done on time

## Getting Started

Notes:

- This repo is a modified version of code-server provided by Coder car, you may find the original repo [HERE](https://github.com/cdr/code-server)

- The software is compiled in a docker container, which means Docker is required to be installed in your host machine
- The data associated with the container will be preserved in `/appdata/code-server` in your local machine

To install, run:

```bash
$ docker run -d --name code-server \
  -v /appdata/code-server:/data \
  -p 8443:8443 \
  --privileged \
  --restart unless-stopped \
  hikariai/code-server:latest
```

*** The Web UI will be available at `http://localhost:8443`

## Pre-installed Softwares

- Python v3.6.9
- Node v12.20.0
- Npm v6.14.8

## Version

| version |             Updates             |
| :-----: | :-----------------------------: |
| latest  | Pre-installed softwares updated |
| v1.0.0  |     First launched version      |

You may find all the version [HERE](https://hub.docker.com/repository/docker/hikariai/code-server/tags?page=1&ordering=last_updated)

## Reference

[Orignal code-server repo from cdr/coder-server](https://hub.docker.com/repository/docker/hikariai/code-server/tags?page=1&ordering=last_updated)

## License

[MIT LICENSE](https://github.com/yqlbu/code-server/blob/main/LICENSE)
