---
STATUS: example
OWNER: 技术负责人
UPDATED: 2026-05-22
---

# 本地开发、测试、部署引导

## 环境要求

| 工具 | 版本 | 说明 |
| --- | --- | --- |
| Node.js | 20+ | 前后端运行环境 |
| pnpm | 9+ | 包管理 |
| PostgreSQL | 15+ | 本地数据库 |

## 初始化

```bash
pnpm install
cp .env.example .env
pnpm db:migrate
```

## 本地启动

```bash
pnpm dev
```

## 常用命令

| 命令 | 用途 |
| --- | --- |
| `pnpm dev` | 启动本地服务 |
| `pnpm test` | 运行测试 |
| `pnpm lint` | 代码检查 |
| `pnpm db:migrate` | 执行数据库迁移 |

## 测试

```bash
pnpm test
pnpm lint
```

## 配置与密钥

- 配置文件：`.env`
- 环境变量：`DATABASE_URL`, `SESSION_SECRET`
- 密钥管理：生产环境通过部署平台密钥管理，不提交到仓库。

## 部署

| 环境 | 命令/流程 | 备注 |
| --- | --- | --- |
| 开发 | `pnpm deploy:dev` | 自动部署到开发环境 |
| 测试 | `pnpm deploy:staging` | 发布前验证 |
| 生产 | CI 手动审批后部署 | 保留回滚版本 |

## 故障排查

| 问题 | 可能原因 | 解决方式 |
| --- | --- | --- |
| 数据库连接失败 | `DATABASE_URL` 错误 | 检查 `.env` 配置 |
| 登录后跳转失败 | `SESSION_SECRET` 缺失 | 补充环境变量 |

