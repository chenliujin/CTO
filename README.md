# Docker
- 私有镜像仓库
- image
 - nginx-php-fpm
 - redis
 - mosquitto
 - mysql
 - nodejs
 - go

---

# kubernetes
- 滚动升级
- 资源限制
- 自动伸缩
- 容器健康检查
- 集群监控

---

# 服务器架构设计(腾讯云)

- 网络架构设计
 - 组网：公网网关 + 内网 共享上网

# MySQL
- 主从同步

---

# 服务器迁移（阿里云迁移到腾讯云）

## 图片迁移
- 构建隧道迁移阿里云内网的图片

## 数据库迁移
- 主从同步
- 锁定主库，让从库完全同步
- 从库切换为主库

## redis 迁移







搭建MYSQL高可用主主负载集群，keepalived+haproxy+mysql

# TODO
- TCP/IP 协议
- 分布式事务
- lvs: dr 模式
- haproxy
- keep alived
- squid: 反向代理
- varnish
- DNS: Bind
