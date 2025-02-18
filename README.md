# 仓库使用指南
## Github Action构建Pages
1. Fork本仓库
2. 前往`Settings - Pages` 选择Github Actions
3. 等待部署完成就可以在`https://<username>.github.io/<reponame>/`预览


## 本地部署方式
1. Linux用户使用如下命令下载mdbook mdbook-katex mdbook-admonish二进制包：
```shell
mkdir bin
curl -sSL https://github.com/rust-lang/mdBook/releases/download/v0.4.45/mdbook-v0.4.45-x86_64-unknown-linux-gnu.tar.gz | tar -xz --directory=bin
curl -sSL https://github.com/lzanini/mdbook-katex/releases/download/0.9.2-binaries/mdbook-katex-v0.9.2-x86_64-unknown-linux-gnu.tar.gz | tar -xz --directory=bin
curl -sSL https://github.com/tommilligan/mdbook-admonish/releases/download/v1.19.0/mdbook-admonish-v1.19.0-x86_64-unknown-linux-gnu.tar.gz | tar -xz --directory=bin
```

2. 使用如下命令构建，并运行在本地：
```shell
bin/mdbook-admonish install
bin/mdbook build
bin/mdbook serve
```
