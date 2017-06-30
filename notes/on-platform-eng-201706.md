
author: @nkchenz
date: 2017/6/29

# On Platform Engineering

## Objectives
- 服务自助化: 去除瓶颈，赋能开发者
- 信息透明化: 系统状态随时掌握, bridge console 可以看到一切
- 运维智能化: 简单故障自愈，高容错，人工旁路检测


## Key Points
Data, Security, Capacity, Performance


## Layers
Data, Bussiness, Presentation

Workloads, Resources, Reliables, Hardwares


## Core Challenges
- 稳定与变化
- 规模与可靠性


## Misc
系统级隔离，服务化，专业级生命周期管理

所有服务都必须是可迁移的，而且是标准迁移方案

会自动更新的系统才是安全的系统，软件是一个有机体

真正的方案往往简洁到简陋，可靠到粗糙

错误的工具，复杂的系统是痛苦之源

将业务逻辑从底层计算资源中解放出来，专注于产品的实现，这是分工的逻辑。提供次时代的工具，是最终目的

因为资源永远都是短缺的，要确保达到最大价值，除了充分考究，精简，别无他法。决定做什么，往往非常重要。
如果抛却过程，市场只看结果，不看过程


## Others

### Patterns


### Basic principles for achieving high availability
- Redundancy
- Contingency plans
- Procedure

from [MySQL High Availability 2nd Edition P124]


### 数据丢失问题
其实数据可靠性是一个写入速度的问题。考虑如下几种方案:
- 彻底刷入磁盘再返回
- 写入 journal log 再返回
- 写双份机器再返回 replication 
- 写多份机器再返回 raft 协议
- 做成石刻备份

业务上的事务与 mysql transaction

三种复制方式:
- async replication
- semisync replication
- raftsync replication

### What makes a good engineer

Curiousity & Urge, 内在渴望了解整个系统怎样工作，这种不可抑制的 urge, make the difference

勤能补拙，两者必有其一。伤害 + 血槽 

从业人员应该接受工程实践的培训，不同工种需要具备不同的素质: 理解复杂系统的能力，提出解决方案的能力，实现标准的能力，运维保障的能力

