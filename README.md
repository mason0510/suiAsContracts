# moveAs

# sui-move 文档
论坛搭建视频
https://www.bilibili.com/video/BV1ME411g7hs/


第一个sui合约开发
https://ja99-doge.github.io/2022/12/10/sui_smart_contract/



move社区开发
https://move-china.com/


move案例
https://706community.notion.site/Move-Demo-3f3a5640ea054d1fae17b84f617d7a34

sui开发文档大全
https://shimo.im/file-invite/Ce6DHkFDR28bt2kw8X3VmX5lmg046/ 猴子 邀请您协作《sui-move开发文档大全》，点击链接开始编辑


无服务器
https://app.netlify.com/drop


前端
sui 连接钱包示例
https://wallet-kit-demo.vercel.app/
https://github.com/suiet/wallet-kit/fork


前端例子
https://juejin.cn/post/7017707698284134414
https://github.com/mason0510/reactRouterDemo

实现
https://kit.suiet.app/docs/QuickStart


交易所兑换
https://www.arayafi.org/swap



sui-move开发文档大全


分割线
----------------------------------------------------------------------------------------------------------------------------

immo研究
质押合约
https://explorer.celo.org/mainnet/address/0xA02F4e8dE9A226E8f2F2fe27B9b207fC85CFEED2/transactions#address-tabs



算法稳定币研究
https://zhuanlan.zhihu.com/p/342238531
某些机制直接来自于学术论文，如果能够设计出足够优秀的机制，可能引发算法稳定币的应用。此外，在算法稳定币的LP token挖矿阶段，特别依靠博弈论相关的专业知识，普通用户在初始时可用稳定币参与
铸造A需要消耗稳定币B与平台币C. 创世阶段只需要消耗USDC
初始时抵押率为100%，即全部使用USDC抵押铸造FRAX. 1:1
若FRAX价格大于1美元，则降低抵押率,解锁资产, 降低抵押率的目的是为了让FRAX价格回归1美元
若FRAX低于1美元则升高抵押率,锁定资产, 降低抵押率的目的是为了让FRAX价格回归1美元
由于稳定币的稀缺,抵押率下降。 铸造出来的一部分不锁仓。
由于价格下跌。导致不足1美元
FRAX的供应量已经达到7600万，抵押率也降至88.75%，这意味着铸造FRAX需要消耗11.25%的FXS，FXS的价格也回到了7美元

铸造稳定币FRAX需要消耗稳定币USDC和治理代币FXS


bs Cash
Bssis Cash fork自因监管而关闭的一个项目Basis，Basis Cash将其权益代币独立了出来，此外还保留了债券，因此协议中共包含三种代币，Basis Cash（BAC）、Basis Share（BAS）和Basis Bond（BAB），其中BAB是不可转移的。
Basis Dollar与Mith Cash受到的关注最多，它们相比Basis Cash只是修改了部分参数。比如Mith Cash在前期MIC的产出中，将矿池数量增加到了16个。
稳定币池除了常用的法币抵押型稳定币外，还增加了算法稳定币ESD、BAC、FRAX；社区池除了项目方自己的MITH以外，还有YFI、COMP、LINK、AAVE等其它7种DeFi代币。


ESD
在ESD发行的前30天，ESD的价格预言机被设定为1.1USDC，在这期间，ESD的供应量每8小时增加10%。ESD的早期参与者获得了上百倍的收益。

Ampleforth
所有算法稳定币里最知名的一个。
rebase时参考的价格以过去24小时的成交量加权平均价为准，当该价格高于1.05美元时，所有用户钱包中的AMPL余额同时增加；价格低于0.95美元时，所有用户的AMPL余额同时减少。


结合四种算法稳定币的特点，我们可以得出以下结论：

一个最优的算法稳定币方案可能需要结合四种算法稳定币的优缺点，并进行一些修改。

首先，可以采用供应量自动调整机制来维持稳定币的价格稳定性，这样可以避免由于人为干预导致的价格波动。

其次，可以引入锁仓机制来限制供应量的增长，并在锁仓期结束后按照一定的比例释放。
锁定部分流动性。

第三，可以加入额外的机制来维护稳定币的价格，如对稳定币流通性进行限制或者对长期锁仓的用户进行奖励。

最后，可以采用多种数据来指导调整策略，如采用成交量加权平均价或者采用市场平均价等。

总的来说，这种算法稳定币方案应该能够有效维持稳定币的价格，同时避免了各种算法稳定币的缺陷。
。
1.引入风险管理机制: 为了防止价格过度波动,可以引入风险管理机制,当价格出现异常波动时,自动调整供应量来维持稳定.

2.透明化: 为了让用户能够了解稳定币的运作机制,可以透明化稳定币的数据,如供应量,锁仓量,价格等.

3.灵活性: 为了调整策略更灵活,可以采用更多种数据来指导调整策略,如采用成交量加权平均价或者采用市场平均价等,并且支持社区投票来决定调整策略

4.稳定基金: 为了应对市场波动,可以引入稳定基金来维护稳定币的价格.

5.可持续性: 稳定币的发行应该满足可持续性,避免对环境造成不良影响.


定义一个稳定币合约，用来维护稳定币的状态，如供应量，锁仓量等。

实现供应量自动调整机制，当价格出现异常波动时，自动调整供应量来维持稳定。

实现锁仓机制，限制供应量的增长，并在锁仓期结束后按照一定的比例释放。

实现风险管理机制，如对高度流通的稳定币进行销毁或者对长期锁仓的用户进行奖励。

实现透明化，让用户能够了解稳定币的运作机制,可以透明化稳定币的数据,如供应量,锁仓量,价格等.

实现灵活性,支持社区投票来决定调整策略,采用成交量加权平均价或者采用市场平均价等.


stake/bond-rebase-unstake


# 编译
稳定币项目
sui move build --skip-fetch-latest-git-deps 
