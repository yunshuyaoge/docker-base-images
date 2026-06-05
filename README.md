# docker-base-images

Docker 基础镜像仓库，提供各种常用服务的基础镜像。

## 目录结构

```
docker-base-images/
├── alpine-mariadb/      # Alpine + MariaDB 镜像
├── alpine-nginx/        # Alpine + Nginx 镜像
├── alpine-redis/        # Alpine + Redis 镜像
├── node/                # Node.js 镜像
└── README.md
```

## 镜像列表

| 镜像名称 | 描述 | 状态 |
|----------|------|------|
| node | Node.js 运行时镜像 | ✅ |
| alpine-mariadb | Alpine Linux + MariaDB | 🔄 |
| alpine-nginx | Alpine Linux + Nginx | 🔄 |
| alpine-redis | Alpine Linux + Redis | 🔄 |

## 使用方法

每个镜像目录下都包含 `Dockerfile` 和相关配置文件。

```bash
# 构建镜像
cd <镜像目录>
docker build -t <镜像名称>:<版本> .

# 运行容器
docker run -d <镜像名称>:<版本>
```

## 贡献

欢迎提交 PR 添加新的基础镜像。

## License

MIT
