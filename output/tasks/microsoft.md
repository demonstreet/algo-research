# 微软公司广告业务与广告算法发展历程

## 一、门户时代：MSN 与第三方广告依赖（1995—2005）

微软的广告业务根植于其在线服务战略。1995年8月，随 Windows 95 发布的 The Microsoft Network（MSN）最初是一款订阅制拨号上网服务，与 AOL、CompuServe 竞争。1998年，微软将 MSN 重塑为免费门户网站 msn.com，与 Yahoo、AOL 正面交锋。同年收购 Hotmail（1997年12月完成），1999年推出 MSN Messenger，门户流量迅速增长。1998年数据显示，MSN 用户触达率一年内增长59%，广告收入同比增长超过300%，并与 First USA、Unilever 等签署近1.6亿美元的大型广告协议。

这一时期，微软尚未建立自主搜索广告体系。MSN Search 的付费广告长期由 Overture（后被 Yahoo 收购）供应，微软仅分得部分收入。门户展示广告则依赖传统品牌合约与内容合作，广告主需与微软销售团队洽谈打包方案，缺乏像 Google AdWords 那样的自助竞价平台。微软内部已意识到搜索营销的价值，但自主广告技术尚未成熟。2000年前后，MSN 经历多次改版与巨额营销投入——全国电视广告、CD 促销、电脑购买返利等——累计投入逾25亿美元，门户定位逐渐清晰：以 Hotmail、Messenger 等高频服务聚合流量，再通过广告变现。MSN 高管 Mehdi、Cole 等人推动以客户为中心的产品整合，为后续 adCenter 建设奠定组织基础。

## 二、自主平台建设：adCenter 与收购整合（2005—2010）

2005年3月，微软在 MSN Strategic Account Summit 上宣布 adCenter 战略，2006年5月由 CEO 史蒂夫·鲍尔默正式发布 Microsoft adCenter，在美国市场承担 MSN Search 100% 付费搜索流量。该项目由 MSN 总经理 Tarek Najm 主导，目标是让广告主一站式购买搜索、情境与展示广告。2006年6月，微软与 Yahoo 的广告供应合约到期，MSN Search 全面切换至 adCenter 广告。

为补齐能力短板，微软同期展开密集收购：2006年收购 DeepMetrix 发展 adCenter Analytics；2007年以约60亿美元收购数字营销公司 aQuantive（当时微软最大收购案之一，旨在对标 Google 的 DoubleClick）；同年收购 ScreenTonic、AdECN，2008年收购 YaData。这些资产共同构成微软广告技术栈的早期基础，覆盖分析、展示、程序化交易与数据能力。adCenter 同期还推出 pubCenter 发布商平台，形成"Microsoft Advertising"品牌下的广告主—发布商双边市场雏形。

2010年1月，微软与 Yahoo 达成 Microsoft Search Alliance（搜索联盟）：微软接管 Yahoo Search 运营，并通过合资平台统一销售 Bing 与 Yahoo Search 广告。2010年10月，全部 Yahoo 赞助搜索客户迁移至 adCenter。同年，微软推出 Bing 搜索引擎（2009年正式发布），取代 MSN Search / Live Search 品牌。搜索与广告体系开始深度融合。

## 三、算法突破：AdPredictor 与竞价智能化（2009—2015）

广告算法的里程碑是 AdPredictor。2009年夏，由微软剑桥研究员 Joaquin Quiñonero Candela 团队开发的贝叶斯在线学习算法全面替代 Bing 旧 CTR 预测系统，驱动全部赞助搜索流量。AdPredictor 基于广义线性模型与 probit 链接函数，采用因子化高斯信念分布与近似消息传递，实现特征级自动学习率调整、在线增量学习与探索—利用平衡。其核心任务是在关键词拍卖中预测每次展示的点击概率，进而决定广告排序与计费。

AdPredictor 使 Bing 倾向于展示更少但相关性更高的广告（第三方统计 Bing 平均约3.85条/关键词，低于 Google 的5.72条），提升了用户体验与广告主效率。此后，微软持续演进自动竞价策略：Maximize Clicks、Maximize Conversions、Target CPA、Target ROAS 等，由后端模型实时计算关键词出价，结合 Universal Event Tracking（UET）转化数据优化投放。

2012年9月，adCenter 更名为 Bing Ads，搜索联盟更名为 Yahoo! Bing Network。2015年，Yahoo 合作调整：微软成为 Bing 搜索广告的独家销售方；AOL 接管微软在九国的展示/移动广告销售，AOL 站点改用 Bing 搜索与 Bing Ads。广告业务在联盟博弈中持续整合。

## 四、生态扩张：LinkedIn、Audience Network 与 Xandr（2016—2022）

2016年6月，微软宣布以262亿美元收购 LinkedIn，12月交易完成。收购初期即规划将 Sponsored Content 扩展至微软全系产品，并打通 Office、Dynamics 等企业场景。LinkedIn 自身广告系统采用实时拍卖机制：出价与相关性评分共同决定展示，相关性由机器学习模型（后演进为 LiRank 等大规模排序框架）预测 CTR 与转化概率。LinkedIn 的 CTR 模型从 GLMix 迁移至深度学习架构，引入 shallow tower 缓解过度预测，实现约8.5% CTR 提升；竞价代理采用随机最优控制框架，在 GSP 与一价拍卖中平衡预算与 ROI。

2018—2019年，微软将 LinkedIn 职业数据引入搜索广告：LinkedIn Profile Targeting 允许按公司、行业、职能在搜索、动态搜索与购物广告中叠加出价调整（bid modifier 模式，不缩小受众范围），成为相对 Google 的差异化 B2B 能力，初期仅限美国市场。LinkedIn 广告拍卖本身亦持续演进：从 GLMix 到深度学习 CTR 模型，再到 2024年 LiRank 工业级排序框架（融合 DCNv2、ID embedding、等渗校准层），在广告、职位推荐等多场景带来显著转化提升。2018年，Microsoft Audience Network（MSAN）上线，整合 Microsoft Graph 数据与 AI，在 MSN、Outlook、Microsoft Edge 等自有库存及合作站点投放原生广告，成为 2019 年品牌重塑的重要支撑。

2019年4月，Bing Ads 正式更名为 Microsoft Advertising，回归"微软广告"品牌，反映业务已从单一搜索扩展至搜索、原生、程序化与零售媒体全链路。同年，微软成为 Verizon Media（含 Yahoo、AOL）独家搜索广告提供商，MSAN 获得 Verizon 库存接入。

2021年12月，微软宣布从 AT&T 收购程序化广告平台 Xandr；2022年6月交易完成。Xandr Invest（DSP）与 Xandr Monetize（SSP）与 MSAN、PromoteIQ 等整合，强化第一方数据驱动的开放网络投放能力，MSN、Outlook 等自有库存可直接通过 Xandr SSP 变现，应对 Cookie 淘汰与隐私监管趋势。

## 五、AI 时代：Performance Max、Copilot 广告与 Copilot 助手（2023—至今）

2023年7月，微软推出 Performance Max（PMax）开放测试，2024年3月全球上线。PMax 是 AI 驱动的跨渠道自动化广告类型：广告主设定目标、预算、素材与受众信号，微软 AI 在搜索、原生、MSN、Copilot 等全网络_inventory 中动态组合素材与定向，实现无关键词列表的智能投放。支持从 Google Ads 导入 PMax 活动，平均 ROAS 提升显著。

2024年起，Copilot 成为广告新场景。Performance Max 活动默认有资格在 Copilot 对话搜索中展示，广告标注"Sponsored"标签。微软称 Copilot 搜索广告在相关性指标上较传统搜索高约25%，转化率高约76%，CTR 高约73%。2025年，微软在 Advertising Accelerate 活动上推出 Showroom Ads：分屏沉浸式体验，一侧为品牌 AI 导购（如奔驰试点），另一侧为 Copilot 追问；另有"广告语音"解释推荐逻辑、品牌定制 AI Agent 等形态。Mercedes-Benz Showroom Ads 试点显示，Copilot 互动用户购买意愿较 Bing 搜索高约53%。

与此同时，微软在广告平台内嵌 Copilot 助手（2024年广泛推出，支持16种语言），免费提供活动诊断、绩效快照、素材生成与自然语言活动管理，将生成式 AI 嵌入广告主工作流。Connected TV、视频素材 AI 生成等功能同步扩展。

## 六、总结与趋势

纵观近三十年，微软广告业务经历了"流量门户—第三方依赖—自主平台—生态并购—AI 原生"的演进路径。算法层面，从规则匹配到 AdPredictor 贝叶斯 CTR 预测，再到深度学习排序（LinkedIn LiRank）、自动竞价与 PMax 端到端优化，技术深度持续加深。业务层面，从 MSN 展示合约到 Bing 搜索联盟，再到 LinkedIn B2B、Xandr 程序化与 Copilot 对话广告，_inventory 与数据资产不断扩张。

当前，微软广告仍居全球搜索广告第二位，份额远逊于 Google，但凭借 Edge/Copilot 生态、LinkedIn 职业数据、MSAN/Xandr 开放网络及通常低20%—35%的 CPC，在 B2B、零售与 AI 搜索新兴场景中形成差异化。2025财年，微软搜索与新闻广告收入同比增长约21%，虽仍落后于 Meta 与 Google，但增速可观。平台还提供 Sponsored Products（零售制造商商品推广）、Connected TV 广告、购物受众活动等多元产品。未来竞争焦点将落在：对话式搜索中的原生广告体验（Showroom Ads、品牌 Agent）、第一方数据隐私合规下的定向精度，以及跨 Microsoft 365、LinkedIn、Bing/Copilot 的统一 AI 投放平台能力。广告算法将从单次 CTR 预测，进一步走向全旅程转化优化与多模态创意生成的一体化智能投放。
