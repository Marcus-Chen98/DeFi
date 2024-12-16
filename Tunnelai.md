---
timezone: Asia/Shanghai 
---
---

# {唐三水}

1. 自我介绍
 矿池Web2研发，探索Web3
2. 你认为你会完成本次残酷学习吗？
 会
## Notes

<!-- Content_START -->

## 稳定币
### 2024.08.19
#### 稳定币的历史
1、为什么需要有稳定币
 * 大部分虚拟资产需要稳定资产作为会计核算、也是退出头寸的避风港。稳定资产通常使用美元。
 * 直接使用美元的劣势
   * 银行间转账的费用成本和时间成本
     * 区块链 24小时，银行有假期、人工各种因素
     * 银行跨国汇款成本高，且受各国管控影响较大

2、早期的稳定币代表
 * BitUSD
   * 抵押物：加密货币
 * NuBits
   * 算法稳定币，利用算法自动调节稳定币的供应，以维持其价格挂钩。
 * Tether代币： USDT
   * 法定货币抵押稳定币


### 2024.08.20
2、早期的稳定币代表
 * BitUSD
   * 抵押物：加密货币
 * NuBits
   * 算法稳定币，利用算法自动调节稳定币的供应，以维持其价格挂钩。
 * Tether代币： USDT
   * 法定货币抵押稳定币

### 2024.08.21
3、稳定币的类型
 * 链下质押稳定币
   * 法定货币质押
     * USDT
     * USDC
   * 商品质押
     * PAX Gold (每个 pax 代币都由一金衡盎司的 400 盎司金条支持)
   * 风险：
     * 受挂钩资产健康状况影响
     * 监管风险
     * 交易对手风险
     * 质押公司透明度
 * 加密质押稳定币
   * 质押加密货币
   * 优势：
     * 无需信任第三方
     * 不受审查和监管
     * 透明度高，用户可以完全依赖智能合约的代码来确保其安全性和透明度
   * 劣势：
     * 挂钩维持较为困难，且需要超额抵押，导致资本效率低下。
 * 算法稳定币
   * 算法自动调节稳定币的供应，以维持其价格挂钩。采用铸币税的方式，
   * 代表： UST/LUNA, ESD, Basic Cash, FRAX
   * 优势：
     * 资本效率高，不需要抵押品，理论上可以有效维持挂钩。
   * 劣势：
     * 由于算法机制的复杂性和市场信心的波动，算法稳定币的风险极高。UST 的崩盘事件说明了这一类型稳定币存在的巨大风险。

reference: 
1. https://banklessdao.substack.com/p/the-stablecoin-edition-defi-download
2. https://nigdaemon.gitbook.io/how-to-defi-advanced-zhogn-wen-b/di-6-zhang-qu-zhong-xin-hua-de-wen-ding-bi-he-wen-ding-zi-chan

### 2024.08.22
#### MakerDAO
1、MakerDAO介绍

MakerDAO 是一个建立在以太坊区块链上的去中心化自治组织（DAO），其核心目的是通过创建和管理一种去中心化的稳定币 DAI，提供一种稳定的价值存储方式。以下是对 MakerDAO 的详细介绍：

 1. **去中心化自治组织（DAO）**
   - MakerDAO 是一个由持有 MKR 代币的社区成员共同治理的去中心化自治组织。持有者可以通过投票决定系统的关键参数和治理提案，比如稳定费率、抵押类型等。
   - 这种治理模式确保了系统的去中心化，任何一个单一实体都无法单独控制系统。

 2. **DAI 稳定币**
   - MakerDAO 的核心产品是 DAI，一种去中心化的、与美元挂钩的稳定币。与许多其他稳定币不同，DAI 并非由中心化的实体通过法币储备支持，而是通过超额抵押的加密资产生成的。
   - 用户可以通过将加密资产（如 ETH、WBTC 等）作为抵押物锁定在 MakerDAO 的智能合约中，借出相应价值的 DAI 稳定币。

 3. **借贷功能**
   - 用户可以通过 MakerDAO 平台创建一个抵押债仓（Vault），将他们的加密资产作为抵押物，借出 DAI 稳定币。这一功能使得 MakerDAO 成为一个去中心化的借贷协议。
   - 借贷过程中，用户需要维持一定的抵押率，以确保系统的安全。如果抵押物的价值下降，导致抵押率跌破规定的最低标准，系统会自动清算抵押物以偿还借款，保护平台免受坏账影响。

 4. **MKR 代币**
   - MKR 代币是 MakerDAO 的治理代币，持有者可以参与平台的治理决策。MKR 持有者通过投票来决定系统的关键参数，包括稳定费率、抵押资产种类、清算比率等。
   - 除了治理功能外，MKR 还用于在系统发生债务损失时，通过增发 MKR 代币来覆盖损失，确保 DAI 的稳定性。



2、MakerDAO 为什么捕获RWA: 加密资产抵押品的不稳定性

3、MakerDAO 如何捕获RWA：
3.1 法律包装的必要性：
 - 交易对手风险。试想交易对手破产/跑路的案例，MakerDAO  需要保障的是任何第三方（包括基金经理/投资顾问）都没有能力直接控制、支配、转移其巨额资金；
 - 主体资格认证。链上协议或 DAO  组织无法完成合法持有资产需要的客户识别认证（KYC/AML），导致无法合法购买、持有链下资产。同理，也无法持有自身的 IP  资产；
 - 破产清算资格。一旦出现链下资产的违约、破产、清算情形，由于链上协议或 DAO  并不是一个法律主体，无法立即与现实世界的法院、清算机构做交互。那么就需要保障 MakerDAO  有能力通过治理体系以及法律架构，及时行使处置链下资产的权利。
3.2 如何实现法律包装
3.3 如何治理链下法人实体
3.2-3 请去参考链接观看

reference: https://web3caff.com/zh/archives/80903

### 2024.08.23

DAI的价值如何保持稳定？
除了降低MakerDAO作为贷方的风险外，CDP机制有助于将DAI与美元挂钩。MakerDAO还可以投票改变稳定费与DAI储蓄率（在DAi储蓄率智能合约中支付给质押者的利息），以控制DAI的供需。这三大工具共同维持DAI与美元按照1：1的比率挂钩。让我们来看看这究竟是怎么回事：
1.当DAI跌破挂钩比率时，该系统会吸引用户偿还债务、收回抵押品并销毁DAI。这可以通过提高稳定费来实现，让借贷变得更加昂贵。DAO还可以提高DAI储蓄率，扩大代币投资需求。
2.当DAI高于其挂钩比率时，则情况正好相反。如果稳定费降低，DAO将激发DAI的生成。这创造了新的DAI，增加了总供应量，降低了价格。MakerDAO还可以通过降低DAI储蓄率来减少DAI的需求，这意味着投资者会换其他的方式来赚利息。

reference: https://www.binance.com/zh-CN/square/post/43195

### 2024.08.24
## 借贷协议

去中心化贷款可以解决这个问题。它允许任何人获得贷款，仅基于他们钱包中的资产。它全年无休，不会因你的外表而歧视你。每个人都使用相同的参数进行评估，只需几分钟即可完成。
DeFi 的魅力在于，它使获取复杂的金融服务变得像访问互联网一样简单，而且 DeFi 借贷在多个方面优于传统金融借贷：
- 可信的中立性：用户无需通过中心化的第三方机构来抵押资产进行贷款。智能合约可处理包括利率、抵押和清算在内的所有事宜。
- 无需许可：每个人都有相同的贷款渠道，任何人都可以成为贷款人。只要你有资金，你的利率将与地球另一端的人相同。种族、宗教、性别和外貌对你的信誉没有任何影响。
- 速度：用户不再需要等待贷款审批。这加快了贷款发放流程，因为只要用户拥有必要的抵押品，他们就可以借贷。用户借贷所需的唯一东西就是资金和互联网连接。
- 透明度：由于所有交易、资金、合约和活动都在链上，因此每个人都可以看到系统的变化和市场条件的变化。
- 可用性：每天 24 小时都可以通过任何一台连接互联网的计算机访问应用程序。没有银行假期，也无需员工执行交易。
- 税收影响：借贷协议允许用户利用其加密资产的杠杆敞口，而无需在其抵押品上产生应税事件。


### 2024.08.25
### DeFi 借贷基础知识
1、APR 与 APY：
APR ： 年化收益率  Annual Percentage Rate 单利
APY ： 年化收益率 Annual Percentage Yield 复利

2、流动资金池（Liquidity Pools）
流动性池是锁定在智能合约中的代币对或代币组的集合

3、 AMM （Automatic market maker）

AMM 是一种让人在去中心化交易所（DEX）上买卖代币的方式。它跟传统的交易方式不一样，不需要买家和卖家直接匹配。相反，它通过一个叫做**流动性池**的东西来完成交易。

1. **流动性池（Liquidity Pool）**:
   - 想象一个“资金池”，里面有两种不同的代币。比如，你有一个池子里面装着 ETH（以太坊）和 USDC（一个稳定币）。
   - 这个池子里的资金是由用户提供的。用户把他们的代币放进池子里，并因此赚取一些交易费作为回报。

2. **如何交易？**
   - 当你想要用 USDC 买 ETH 时，你不需要找一个愿意卖 ETH 的人。相反，你直接跟这个资金池交易。你把 USDC 放进池子里，池子里的 ETH 会相应减少一些给你。
   - 池子通过一个简单的数学公式来决定 ETH 和 USDC 的价格。这公式确保无论交易量如何，池子里的总价值保持不变。

3. **去中心化和无需许可**:
   - 你不需要通过一个中心化的交易所（比如币安或火币）来交易。任何人只要有钱包就能参与，不需要经过复杂的审核或许可。

为什么 AMM 很重要？

- **简单易用**：AMM 的交易过程完全自动化，用户无需担心买不到或卖不掉，因为他们一直在和资金池交易。
- **无需中介**：所有交易都是在区块链上通过智能合约自动执行的，不需要中介或中间人，这使得交易更安全透明。
- **人人都可以参与**：任何人都可以成为流动性提供者，把自己的代币放到资金池中赚取交易费。


### 2024.08.26

4、稳定费（Stability Fee）
稳定费是对借入资金余额收取的可变年费

5、抵押率 （Collateralization Ratio）
抵押率 = （抵押品价值/债务价值）x 100

6、浮动利率模型 （Variable Interest Rate Model）
利率模型用于确定资产供应商应获得多少报酬以及借款人应为借给他们的资产支付多少报酬。该模型试图平衡三个变量：
- 资金池流动性
- 借贷利率
- 供给率
![image](https://github.com/user-attachments/assets/bcedde11-b679-4813-8dc8-96ea537bfab5)

7.Liquidations  清算
当存入的抵押品价值低于最低抵押率时，借贷平台会自动出售借款人的抵押品以偿还未偿还的债务和可能收取的任何费用或罚款。偿还债务后剩余的任何抵押品都将退还给借款人

### 2024.08.27
8. 闪电贷（todo）
闪电贷允许用户在极短的时间内（同一区块内）无需提供抵押即可借入资产。这些贷款通常用于不同 DeFi 协议之间的套利机会。
不存在资金损失的风险，因为如果贷款未在同一笔交易中偿还，则贷款被视为无效。闪电贷由Aave首创，必须通过定制智能合约申请，该合约在一笔交易中偿还贷款和利息。这些贷款主要面向开发人员，但DeFi saver等工具为最终用户提供了使用这项新技术的途径。

9. 隔离池
隔离池允许任何人为自己选择的任何资产创建借贷市场，并根据他们认为合适的风险状况调整参数，而不会污染协议的其余 TVL。流动性隔离将借贷市场彼此分开，保护安全池免受风险较高的池的影响。

### 2024.08.28
借贷经典项目
1、Maker 
Maker 被认为是第一个 DeFi 项目，并且一直持有最多的 ETH 锁定量。Maker 使用稳定币 DAI 创建抵押债务头寸，允许用户将治理批准的抵押品存入 Maker Vault，从而让债务人能够铸造/借入 DAI。这些借款人为与美元挂钩的 DAI 支付“稳定费”，作为贷款利率。

2、Compound
不懂？ todo



<!-- Content_END -->