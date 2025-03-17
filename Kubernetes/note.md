# 名词解释

## Node 物理机或虚拟机（worker）
### Pod 最小资源调度单元（封装一个或几个docker）
### Service 将一组Pod封装成一个服务，提供统一入口（解决Pod IP 不稳定问题）
### Ingress 管理入口点，针对不同的配置规则访问集群中不同的Service，同时具有负载均衡，域名转发等功能，相当于NGINX
### ConfigMap & Secret 提供运行环境配置文件
### Volumes 共享资源外部挂载卷，实现数据持久化存储
### Deployment 部署无状态应用程序
### StatefulSet 部署有状态应用程序
### kubelet 管理Pod，定期接受Pod规范，反馈信息到ApiServer
### kube-proxy Pod提供网络代理和负载均衡 负责pod和pod间的通信
### container-runtime Pod运行引擎
## Control plane （Controlor）
### apiServer 交互管理集群的关键节点（认证管理）
### etcd key-Value数据库，存储workers中的Node/Pod状态信息数据
### scheduler 调度器，监控集群中所有节点的资源使用情况，调动pod（正常情况下的调度）
### control-manager 监控并管理集群中节点的状态（异常状态下的调度）
### cloud-control-manager 云平台的api，负责与api进行交互

# 环境搭建


