Spring Cloud<br>
Spring Cloud是一系列框架的有序集合。
它利用Spring Boot的开发便利性巧妙地简化了分布式系统基础设施的开发，
如服务发现注册、配置中心、消息总线、负载均衡、断路器、数据监控等，
都可以用Spring Boot的开发风格做到一键启动和部署。Spring并没有重复制造轮子
它只是将目前各家公司开发的比较成熟、经得起实际考验的服务框架组合起来，
通过Spring Boot风格进行再封装屏蔽掉了复杂的配置和实现原理，
最终给开发者留出了一套简单易懂、易部署和易维护的分布式系统开发工具包。
<br>
Spring Cloud Netflix
<br>
与各种Netflix OSS组件集成,组成微服务核心
Netflix Eureka
<br>
服务中心,云端服务发现,一个基于REST的服务,用于定位服务,
以实现云端中间层服务发现和故障转移,是一个服务中心,
服务中心保证稳定性和服务质量
<br>
Netflix Hystrix
<br>
熔断器,容错管理工具,通过熔断机制控制服务和第三方库的节点,
从而对延迟和故障提供更强大的容错能力,有服务故障,需要转移,
服务当机,需要阻止,总进程发生阻塞影响整体计划,Hystrix就可以协调
发现某服务不稳定,可让其下线,或者转移到其他服务
<br>
Netflix Zuul
<br>
Zuul 在云平台上提供动态路由,监控,弹性,安全等边缘服务框架
相当于是设备和Netflix 流应用的web网站后端请求的前门,
阻断非法请求,或者引导请求到对应服务
<br>
Netflix Archaius
<br>
配置管理API,包含一系列配置管理API
提供动态类型化属性,线程安全配置操作,轮询框架,回调机制等功能,
可以实现动态获取配置,原理是每隔60s(默认,可配置) 从配置源读取一次内容,
这样子修改了配置文件后不需要重启服务就可以使修改后的内容生效,
前提使用archaius的API来读取
<br>
Spring Cloud Config
<br>
配置中心,配置管理工具包,可以把配置放到远程服务器,集中化管理集群配置
目前支持本地存储,Git以及Subversion。方便统一管理,升级
<br>
Spring Cloud Bus
事件,消息总线,用于在集群(例如,配置变化事件)中传播状态改变
可以与Spring Cloud Config联合实现热部署,确保各个微服务之间保持消息畅通
<br>
Spring Cloud for Cloud Foundry
<br>
Cloud Foundry ,支持多个框架,语言,运行时环境,云平台以及应用服务
使开发人员可以在很快进行应用程序的部署和扩展,无需担心任何基础架构的问题
<br>
Spring Cloud Cluster
<br>
Spring Cloud Cluster取代 Spring Integration,提供分布式系统中,
集群所需要的基础功能支持,
如: 选举,集群的状态一致性,全局锁,tokens等常见状态模式的抽象和实现
<br>
Spring Cloud Consul
<br>
Consul 是一个支持多数据中心分布式高可用的服务发现和配置共享的服务软件
<br>
Spring Cloud Consul封装了Consul 操作,consul 是一个服务发现与配置工具,
与Docker容器可以无缝集成
<br>
<br>
<br>
Spring Cloud Security
基于 spring security 的安全工具包,给应用程序添加安全控制,
指定不同的服务只能访问特定的资源,保护需要保护的资源
<br>
Spring Cloud Sleuth
日志收集工具包,封装Dapper和Log-based 追踪以及Zipkin 和HTrace操作.
为springCloud 应用实现一种分布式追踪解决方案
<br>
Spring Cloud Data Flow
~ Data flow 是一个用于开发和执行大范围数据处理,
其模式包括ETL,批量运算和持续运算的统一编程模型和托管服务
<br>
~  对于在现代运行环境中可组合的微服务程序来说,Spring Cloud data flow
 是一个原生云可编配的服务,使用Spring Cloud data flow ,开发者可以为像
 数据抽取,实时分析,和数据导入/导出这种常见用例创建和编配数据通道(data pipelines)
~ Spring Cloud Data Flow 是基于原生云对 Spring XD重新设计,
    该项目目标是简化大数据应用的开发,Spring XD 的流处理和批处理模块的重构
    分别是基于 Spring Boot 的stream和task/batch 的微服务程序。
    这些程序现在都是自动部署单元而且他们原生的支持像Cloud Foundry,Apache Yarn
    ,Apache Mesos 和Kubernetes 等现代运行环境
 ~ Spring Cloud Data Flow 为基于微服务的分布式流处理和批处理数据通道
    提供了一系列模型和最佳实践
    





















































































