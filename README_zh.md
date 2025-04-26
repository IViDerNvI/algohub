# AlgoHub

## 快速开始

### 克隆仓库

从 github 克隆仓库，运行以下命令：

```bash
git clone https://github.com/ividernvi/algohub.git
cd algohub
```

### 生成证书文件和私钥

要生成证书文件和私钥，可以使用以下命令：

```bash
cd conf/cert
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout private.key -out certificate.crt
```

此命令将生成一个有效期为 365 天的自签名证书 (`certificate.crt`) 和私钥 (`private.key`)。

### 使用 Docker Compose 运行

确保已安装 Docker 和 Docker Compose。然后运行以下命令：

```bash
cd algohub
docker-compose up -d
```

这将会在容器化环境中构建并启动应用程序。
