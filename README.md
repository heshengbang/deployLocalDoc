# Deploy Document In Your Computer
Because some companys work in LAN or offline environment, there also have some places can't view open-source project's document.
So, you can use this project for deploying document in your personal computer or your LAN serve.Attention, there are some sources are unable, if you find it, you can commit a issue and i will fix it and add it to document.

All images you can get it in hub.docker.com.

# 本地部署开源项目文档
由于某些公司办公是在内网或离线环境，亦或者世界上的某些区域无法访问流行的开源项目的文档。注意，这里有一些资源是得不到的，如果你发现了，请提交一个issue，我会修复并把它加入文档。

所有的镜像都可以在hub.docker.com中得到。

此文档用于帮助在本地或内网环境部署一些流行的开源文档，当前包含以下项目：
- openshift
- revel
- golang
- go-tour
- kubernetes
- docker


# 常用指令

- 构建镜像
`docker build -t docs/kubernetes-docs:v1 . `

- 启动容器
`docker run -p 4000:80 --name kubernetes_docs docs/kubernetes-docs`

- 进入容器
`docker exec -it kubernetes_docs /bin/bash`


# 参考链接

- [Best practices for writing Dockerfiles](https://docs.docker.com/develop/develop-images/dockerfile_best-practices/)
- [Docker —— 从入门到实践](https://yeasy.gitbooks.io/docker_practice/content/)