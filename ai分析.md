结合以下算法稳定币的优点。
1.以Ampleforth为代表的rebase类
Ampleforth是算法稳定币中最具知名度的一个，它通过增加或减少AMPL的供应量，以使AMPL的价格维持在一美元附近。与其它类型的稳定币项目不同，Ampleforth使用rebase操作来整体改变所有用户持有的AMPL。rebase时参考的价格以过去24小时的成交量加权平均价为准，当该价格高于1.05美元时，所有用户钱包中的AMPL余额同时增加；价格低于0.95美元时，所有用户的AMPL余额同时减少。在这个过程中，用户持有的AMPL在供应量中的占比并不会发生变化。
虽然Ampleforth认为当今加密货币存在很强的关联性，通过AMPL的激励方式，可以使AMPL与比特币等加密货币的价格脱钩，从而增强资产的多样性，降低系统性风险。但是，到目前为止，AMPL并没有解决这一问题，并且这反而成了AMPL的缺陷。
2.以Empty Set Dollar为代表的质押锁仓类
ESD的价格稳定性同样基于一种弹性供应模型。当ESD价格高于1美元，协议需要增加供应量时，会铸造新的ESD代币，这些代币会被分给质押者；如果此时系统中有尚未偿还的债务，则会优先偿还这些债务。当ESD的价格下跌时，用户可以选择销毁ESD以优惠价格购买债券，若价格再次高于1美元，债券可以1:1赎回ESD。如果在债券购买后的30天内没有被赎回（价格不足1美元），这些债券将被销毁，对应购买债券的资产将全部损失。
与其它项目不同，Empty Set Dollar还引入了锁仓机制。在系统没有债务的情况下，增发的ESD并不会直接分发给ESD的持有者，而是会奖励给质押ESD以及Uniswap ESD-USDC的LP token的质押者。退出时，ESD与LP token的解锁时间分别为15 epochs和5epochs（每个epoch为8小时）。因为锁定了大量的ESD，在ESD的市值已经达到数亿美元时，外部流通的ESD也极少，这也是ESD被很多人认为是资金盘的原因，这种机制在下跌时很容易造成死亡螺旋。
3.以Basis Cash为代表的多代币类
Bssis Cash fork自因监管而关闭的一个项目Basis，Basis Cash将其权益代币独立了出来，此外还保留了债券，因此协议中共包含三种代币，Basis Cash（BAC）、Basis Share（BAS）和Basis Bond（BAB），其中BAB是不可转移的。BAC是其中的稳定币，锚定1美元；BAS为权益代币，可以分配新铸造的BAC代币；BAB为债券，BAB的价格等于BAC价格的平方，比如BAC为0.7美元时，BAB的价格为0.7BAC（0.49美元）
与ESD一样，当BAC高于1美元时，系统首先允许债券持有者赎回BAC。如果此时还有BAC生成，则以铸币税的形式分配给Boardroom，用户抵押BAS来赚取BAC的每日铸币税。
Basis Cash中的代币以公平的形式分发，一开始向5个稳定币池发放共发放5万BAC，BAS奖励给BAC-DAI和BAS-DAI的Uniswap LP token质押者。
不同的是，Basis Cash分离了稳定币与权益代币，这样BAC将不受权益代币抛压的影响。同样是质押代币收取铸币税，若ESD的质押者要解除质押并在市场上卖出，ESD在二级市场上的价格将会下跌。但在Basis Cash中，BAS的抛售并不会直接影响BAC的价格。这样BAC的价格将会比ESD更加稳定，BAC也更加实用。
4.以Frax为代表的部分算法稳定币
Frax是首个部分算法稳定币项目，在现有算法稳定币的基础上，增加了使用部分稳定币作为抵押资产的概念。Frax中有两种代币，稳定币FRAX和治理代币FXS。铸造稳定币FRAX需要消耗稳定币USDC和治理代币FXS，在创世阶段只需要消耗USDC。初始时抵押率为100%，即全部使用USDC抵押铸造FRAX，之后抵押率每小时调整一次，若FRAX价格大于1美元，则降低抵押率，增加FXS在其中的份额；若FRAX低于1美元则升高抵押率。抵押率每小时调整一次，每次调整0.25%。
按照预期，在上线之后，由于算法稳定币的热度以及FXS的稀缺，抵押率将不断降低，而FXS的价格将不断上涨。而在实际过程中却没有达到预期，其中有一些地方值得思考。
Frax项目有私募，并且会很快解锁一部分，参与不够公平，导致缺乏大资金的入场。
即便如此，FRAX的铸币量也在1小时内超过了2000万美元，但由于存在FRAX-ETH交易对，Frax上线不久后恰逢ETH下跌，导致FRAX被动下跌而不足一美元，抵押率逐渐上升至100%，FXS消耗不足。


dao控制的算法稳定币
由LP和mcUSD支持的算法稳定币为其提供内在价值

投资者
质押 拿celo换取immo 然后生成更多的immo
绑定 提供流动性和这mcUSD在固定归属期后换取打折的immo币

ico募集到的资金100K-usdc
大概10万u 60万人民币
预售:
40K usdc
1k immo
每一个usdc可以换取40musd
生成80k价值的LP
6k被绑定到支持immo供应
20k审计费用
19.7K 营销费用

抵押获取rebase奖励,奖励来源于债券销售的收益.




质押余额超过价格的下跌。
质押是 锁定immo获取sImmo,可以用到其他的defi项目中去
接触质押时销毁simmo获取Immo。当期的rebase奖励没有了。

绑定
协议销售打折的债券获取资产 期末获取奖励的immo币

博弈论
抵押加上绑定是最佳的策略

每一个immo币都有一个对应的mcUSD币支持。

奖励率
分配给每一个rebase质押的immo相对于总供应量的百分比。 分钱的比例。


合约
https://docs.immortaldao.finance/ecosystem/contracts

immo
供应无上限
每一个纪元结束 以设置的奖励铸造immo币 分配给利益相关的人

购买债券时 会铸造 结束时释放.










