# editor-server-side
  
This is an online **editor** that uses **server-side compilers**.  
  
![editor-server-side](preview.gif "editor-server-side")

I am using some well-known frameworks such as *websockets*, [dockerode](https://www.npmjs.com/package/dockerode) or [monaco-editor](https://microsoft.github.io/monaco-editor/) in this project.  
You can adapt any compiler or programming language as you wish.

## installation

Install [node.js](https://nodejs.org/en/download/), [docker](https://www.docker.com/products/docker-desktop) and all [dependencies](package.json).
  
```
npm install
npm start
```
    
## container configuration

Install [docker](https://docs.docker.com/get-docker) and customize the configuration file `docker/Dockerfile`.

```
docker build -t <name> - < docker/Dockerfile
docker run <application> -h
```

Upload your tagged image to registry [docker hub](https://hub.docker.com/).

```
docker login -u <username>

docker tag <name> <username>/<name>
docker push <username>/<name>
```
