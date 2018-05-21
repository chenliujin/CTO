# Docker
- 私有镜像仓库（registry）
- Dockerfile

---

# kubernetes
- 滚动升级
- 资源限制
- 自动伸缩
- 容器健康检查
- 集群监控

---

# 架构设计(腾讯云)

## 网络架构
 - 组网：公网网关(100M) + 内网 共享上网

## MySQL
- 主从同步

## Redis
- 主从同步

## Notice
- 25端口解封(SMTP)

---

# 服务器迁移（阿里云迁移到腾讯云）

## 图片迁移
- 构建隧道迁移阿里云内网的图片

## 数据库迁移
- 主从同步
- 锁定主库，让从库完全同步
- 从库切换为主库

## redis 迁移
- 主从同步

---

# 运维

## ansible
- playbook

---






搭建MYSQL高可用主主负载集群，keepalived+haproxy+mysql

# TODO
- 分布式文件系统
- TCP/IP 协议
- 分布式事务
- lvs: dr 模式
- haproxy
- keep alived
- squid: 反向代理
- varnish
- DNS: Bind

# 开发和测试工具

| 名称 | 提供商/国别 |
| --- | --- |
| Atom | GitHub |
| Selenium | thoughtworks |
| Docker | Docker,Inc. |
| GitLab | GitLab Inc. |
| Appium | United States of America |
| Visual Studio Code | Microsoft |
| PlantUML | United States of America |
| Balsamiq Mockups | Balsamiq Studios |

