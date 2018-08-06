# Apriori
Apriori algorithm is a frequent item-set algorithm for mining association rules. Its core idea is to mine frequent item-sets 
through two stages, namely candidate set generation and downward close-detection of plots

Apriori算法是一种用于关联规则挖掘（Association rule mining）的代表性算法。关联规则挖掘是数据挖掘中的一个非常重要的研究方向，也是一个由来已久的话题，
它的主要任务就是设法发现事物之间的内在联系。

关联规则应用：

1. Apriori算法应用广泛，可用于消费市场价格分析，猜测顾客的消费习惯，比如较有名的“尿布和啤酒”的故事；

2.网络安全领域中的入侵检测技术；

3.可用在用于高校管理中，根据挖掘规则可以有效地辅助学校管理部门有针对性的开展贫困助学工作；

4.也可用在移动通信领域中，指导运营商的业务运营和辅助业务提供商的决策制定。

关联规则算法的主要应用是购物篮分析，是为了从大量的订单中发现商品潜在的关联。其中常用的一个算法叫Apriori先验算法。

关联规则（association rule）：是形如 X → Y 的蕴含表达式，其中X和Y是不相交的项集，即：X∩Y=∅。关联规则的强度可以用它的支持度（support）和置信度（confidence）来度量。

支持度：一个项集或者规则在所有事物中出现的频率，确定规则可以用于给定数据集的频繁程度。σ(X):表示项集X的支持度计数

项集X的支持度：s(X)=σ(X)/N；规则X → Y的支持度：s(X → Y) = σ(X∪Y) / N  

通俗解释：简单地说，X==>Y的支持度就是指物品集X和物品集Y同时出现的概率。

概率描述：物品集X对物品集Y的支持度support（X==>Y）=P（X n Y）

置信度：确定Y在包含X的事务中出现的频繁程度。c(X → Y) = σ(X∪Y)/σ(X)

通俗解释：简单地说，可信度就是指在出现了物品集X 的事务T 中，物品集Y 也同时出现的概率有多大。

概率描述：物品集X对物品集Y的置信度confidence（X==>Y）=P（X|Y）

期望置信度（Expected confidence）

定义：设W 中有e ％的事务支持物品集B，e ％称为关联规则A→B 的期望可信度度。

通俗解释：期望可信度描述了在没有任何条件影响时，物品集B 在所有事务中出现的概率有多大。

概率描述：物品集A对物品集B的期望置信度为support（B）=P（B）

提升度（lift）
定义：提升度是可信度与期望可信度的比值

通俗解释：提升度反映了“物品集A的出现”对物品集B的出现概率发生了多大的变化。

概率描述：物品集A对物品集B的期望置信度为lift（A==>B）=confidence（A==>B）/support(B)=p(B|A)/p(B)



