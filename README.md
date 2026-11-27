# One Time Secret for TerraMaster TOS

用于 TerraMaster TOS 的容器应用说明与发布准备材料。

## 应用信息

- 上游项目：https://docs.onetimesecret.com
- Docker 镜像：`onetimesecret/onetimesecret:latest`
- 架构：linux/amd64、linux/arm64（已通过 Docker Hub 多架构标签核验）

## 运行示例

```bash
docker compose up -d
```

编排包含 Redis 依赖，服务监听容器 3000 端口；部署前请将 `SECRET` 替换为本地随机值。仓库不包含密码、令牌或私钥。

- x86_64 预检截图：`precheck-screenshots/one-time-secret/x86_64/reprecheck.png`
- NAS x86_64 实测：HTTP 200，首页显示 “Keep sensitive info out of your email and chat logs.”

## 状态

- 本地说明材料已准备。
- TerraMaster 审核：未提交。
- 本仓库仅用于应用说明与打包准备。
