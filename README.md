# Furion #
## 概述 ##
在公司内部分布式环境中，会有相当多的 RPC 调用的场景，针对几十、成百、上千的服务器集群，相互之间的调用，很多情况下都是使用 DNS 服务来解析应用地址，但使用 DNS 有 TTL 影响，在某些情况下，项目组内系统需要临时修改一下解析，通知 DNS 维护人员，在时间上也不及时。这时可以使用修改主机本地 hosts 文件来解决。如果公司内部的系统之间的调用都采用本地 hosts 来解析，怎么样呢？

Furion 是一个便利的修改集群 hosts 的工具；可视化、特殊化的管理方式。