# akashic_game_trial

## 1. A long way to install akashic-bmpfont-generator

### 1.1.create docker container for node.js

Dockerfile
```
FROM ubuntu:20.04
```

```
docker build -t hogehoge
```

```
docker run -it hogehoge
```

install dependancy pakage in docker container

```
 $ apt update
 
 $ apt install nodejs
```

confirm installed
```
 # nodejs -v
```

install npm
```
 # apt install npm
```

### 1.2.install canvvas(need for bmpfont-generator)
in the container
```
 # apt update
 # apt install build-essential libcairo2-dev libpango1.0-dev libjpeg-dev libgif-dev librsvg2-dev
 # apt upgrade
 # npm install canvas
```

### 1.2.install akashic-engine
in the container 
```
 # npm install -g @akashic/akashic-cli
 # npm install -g @akashic/akashic-sandbox
 # npm install -g @akashic/bmpfont-generator
```

if error ocuur during npm install, run following command.
```
 # npm install -g npm
```
