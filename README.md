# mydocker
由于某些公司办公是在内网或离线环境，亦或者世界上的某些区域无法访问流行的开源项目的文档。
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