![bannerImage](chess_banner.jpeg)

---
[![Build Status](https://github.com/TeefanDev/Chess/actions/workflows/scala.yml/badge.svg?branch=main)](https://github.com/TeefanDev/Chess/actions/workflows/scala.yml)
[![Coverage Status](https://coveralls.io/repos/github/TeefanDev/Chess/badge.svg?branch=main)](https://coveralls.io/github/TeefanDev/Chess?branch=main)
![RepoSize](https://img.shields.io/github/repo-size/TeefanDev/Chess)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MI)
![Forks](https://img.shields.io/github/forks/TeefanDev/Chess?color=green&style=social)
![Watcher](https://img.shields.io/github/watchers/TeefanDev/Chess?style=social)

---

## Will be changed on new Branch Web-Applications

# How to run Docker container with X11

## Building the Container
```docker build -t chess:v1 .```

## Running the Container
```
xhost +

ip=$(ifconfig en0 | grep inet | awk '$1=="inet" {print $2}')

docker run -e DISPLAY=$ip:0 -v /tmp/.X11-unix:/tmp/.X11-unix -ti chess:v1

xhost -
 ```

---

## Contributors
| [julienco03](https://github.com/julienco03)  |  [TeefanDev](https://github.com/TeefanDev) |
|---|---|
| ![image](https://github-readme-streak-stats.herokuapp.com/?user=julienco03) | ![image](https://github-readme-streak-stats.herokuapp.com/?user=TeefanDev)  |
