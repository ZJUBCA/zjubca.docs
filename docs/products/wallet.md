# ZJUBCA.Wallet

ZJUBCA.Wallet是由协会Wallet组自研的一款基于EOS区块链的移动端钱包。

感谢[@lowesyang](https://github.com/yyh1102) [@awmleer](https://github.com/awmleer)的开发贡献。

感谢花花(凌君华)对Logo与启动页的设计贡献。

[代码仓库](https://github.com/Blockchain-zju/zjubca.wallet)。

## 架构总览
![钱包架构图](http://on-img.com/chart_image/5b5d86e2e4b0be50eac580fe.png)

## 模块详解
### 转账功能
转账功能是钱包的基础功能，可实现基于eosio.token协议发行的token以及基于eosio.nft协议的非同质代币的查询、转账功能。

### 生态服务入口
生态服务入口是协会钱包的信息发布和活动联动的窗口。

该部分分为两个子模块：

- 信息发布模块，由**原生列表**实现。
- 活动联动，即允许第三方的活动报名链接，由**内嵌webview**实现。

#### 信息发布
该模块包含一个信息列表页以及对应的信息详情页。支持分享功能。

#### 活动联动
该模块包含一个活动发布列表页以及一个webview，用于加载活动详情。

活动发布列表可采用非线性，带权重列表，例如轮播图+列表的形式。

### Dapp市场
该模块主要包含三个独立页：

- Dapp浏览器。以Tab的形式切换下面三个页：
	- 市场首页
	- 排行榜
	- 搜索页
- Dapp详情页，主要介绍Dapp的详细信息，并露出启动按钮。
- Dapp运行页（基于WebView）。

Dapp唤起钱包的交易功能遵循社区的[通用对接协议](https://github.com/southex/SimpleWallet)。
