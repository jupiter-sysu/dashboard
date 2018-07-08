## 服务器部署文档
### 服务器基本信息
- CPU:1核
- 内存:2 GB
- 操作系统:CentOS 7.3 64位
- 公网IP:39.108.15.127
- 当前使用带宽:1Mbps

---
### 内网出入方向全部规则
授权策略 | 协议类型 | 端口范围 | 授权类型 | 授权对象  
允许 | 全部 |  -1/-1 | 地址段访问 | 119.132.58.233  
允许 | 自定义 TCP | 5900/5906 | 地址段访问 | 0.0.0.0/0
允许 | 自定义 TCP | 22/22 | 地址段访问 | 0.0.0.0/0
允许 | 自定义 TCP | 23/23 | 地址段访问 | 0.0.0.0/0
允许 | 自定义 TCP | 6379/6379 | 地址段访问 | 0.0.0.0/0
允许 | 自定义 TCP | 443/443 | 地址段访问 | 0.0.0.0/0
允许 | 自定义 TCP | 80/80 | 地址段访问 | 0.0.0.0/0
允许 | 自定义 TCP | 3306/3306 | 地址段访问 | 0.0.0.0/0
允许 | 自定义 TCP | 5432/5432 | 地址段访问 | 0.0.0.0/0
允许 | 自定义 TCP | 1521/1521 | 地址段访问 | 0.0.0.0/0
允许 | 自定义 TCP | 1433/1433 | 地址段访问 | 0.0.0.0/0
允许 | 自定义 TCP | 3389/3389 | 地址段访问 | 0.0.0.0/0


---
### 服务器软件环境
- web:apache
- apache:2.4.10
- php:5.5.7
- mysql:5.6.21

---