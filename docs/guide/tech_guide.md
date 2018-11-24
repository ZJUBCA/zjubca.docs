## 区块链技术入门指南

浙大区块链协会版权所有。

在阅读本指南之前，请写完成[起步](getting_started.md)中的学习项目。

## 底层技术学习

###  基础

- 底层：学习Go语言。[a tour of Go](https://tour.golang.org/welcome/1)。若只希望学习应用层，则可先暂时跳过该步。
  - **熟练使用各种搜索引擎，首选Google，其次百度。**
  - **能够翻墙。**

- 应用层：
  - web相关技术：
    - 前端: html/css/javascript。开发框架:react, react-native等。
    - 后端: Node.js, jsp, python等。
  - 智能合约：C/C++, Solidity, Javascript等。

### 进阶

#### 应用层

- [详解 ERC20 代币及众筹](https://juejin.im/post/5b2359c651882574d73c6dfe)
- 熟练使用EOS桌面钱包Scatter与移动端钱包Meet.one。
- 学习EOS区块链体系架构，熟练使用[EOS区块链交互工具](https://eostoolkit.io/)
- [EOS智能合约开发与源码解析](https://bihu.com/article/293974)
  - [EOS官方卡牌游戏示例](https://github.com/EOSIO/eosio-card-game-repo)
- [以太坊智能合约教程](https://ethfans.org/posts/101-noob-intro)
  - 以太坊私链搭建，自行Google或百度。
  - 智能合约实战：[简单投票合约](https://my.oschina.net/u/2275217/blog/1800103)

#### 底层

底层的学习主要围绕**建立区块链系统的基本架构认知**与**阅读优质项目的源码**。

- [tinychain](https://github.com/yyh1102/tinychain) 一个较为轻量的区块链底层项目，适合熟悉区块链系统的一些常见模块。**该项目目前为私有仓库，请需要的朋友联系LowesYang获取访问权限**。常见模块有：
  - 钱包账户模块：钱包管理器。
  - 共识模块：共识算法的实现。
  - 加密模块：加密算法的实现。
  - core模块：区块链、区块、交易、默克尔树、世界状态等模块的实现。
  - 执行器模块：执行交易、写区块、同步区块等操作。
  - 虚拟机模块：智能合约虚拟机的实现，EVM, WASM-VM，等。
  - 网络模块：节点间的P2P通信。
  - rpc服务模块：区块链系统对外暴露的过程调用(RPC)服务。
  - 数据库模块：存储区块、交易、状态等数据。
  - 隐私保护：数据隐私保护
  - 跨链，二层网络等。。。
- [EOS.IO](https://github.com/EOSIO/eos) EOS区块链官方仓库
  - [白皮书](https://github.com/EOSIO/Documentation/blob/master/TechnicalWhitePaper.md)
  - [EOS合约开发官方文档](https://developers.eos.io/eosio-cpp/docs/introduction)
  - [EOS智能合约开发与源码解析](https://bihu.com/article/293974) 推荐。
- [go-ethereum](https://github.com/ethereum/go-ethereum) 以太坊官方客户端
  - [以太坊wiki](https://github.com/ethereum/wiki/wiki)
  - [以太坊源码分析](https://blog.csdn.net/turkeycock/article/category/7669858)