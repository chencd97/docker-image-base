## Docker Hub
https://hub.docker.com/r/chencd97/base

## 镜像内容

base中所有镜像的源都来自 `ubuntu:latest`

目前只构建 `x86-64` 架构镜像

端口暴露 `无`

持久化目录 `无`

------

### Java jre 镜像

- `ubuntu_jre8u202`

From: [Oracle JDK](https://www.oracle.com/java/technologies/javase/javase8-archive-downloads.html) - jre1.8.0_202

- `ubuntu_ojre11`
- `ubuntu_ojre21`
- `ubuntu_ojre21`

From: [Adoptium OpenJDK](https://adoptium.net/) - [Eclipse Temurin™](https://adoptium.net/temurin/releases/)

镜像均已配置 `JRE_HOME`, `CLASSPATH` 以及系统 `PATH` 变量

您可以直接执行以下命令查看镜像 java 版本

```shell
docker run \
       --rm \
       chencd97/base:[tag] \
       java -version
```
