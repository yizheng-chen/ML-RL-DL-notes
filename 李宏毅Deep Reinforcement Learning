待解决: min(cross entropy) = max(最大似然估计)

## reinforcement learning

Actor 根据环境State作出决定action，决定之后得到reward

一次游戏成为一个episode，计算一个episode的total reward

trajectory tao = { s1,a1,s2,a2,....,sT,aT}

P theta (tao) = p(s1)ptheta(a1|s1)p(s2|s1,a1)theta(a2|s2)...

R(tao) = total reward in one episode （R: random variable 有随机性，计算的是期望）

### Policy Gradient

gradient ascent

Gradient (f(x)) = f(x) gradient (log f(x))

![9E3C42AE-4D66-4811-8EB0-4068234CB91C](/Users/yizhengchen/Library/Containers/com.tencent.qq/Data/Library/Application Support/QQ/Users/229182954/QQ/Temp.db/9E3C42AE-4D66-4811-8EB0-4068234CB91C.png)



训练N次，得到每次的(at,st)pair，然后得到gradient

只能用一次（后面会改进）

**Implementation**

当作是分类问题

input State output Action

Tip1:baseline

解决sampliing中某些情况没有被sampled：

​	R--> R-b，让这一部分有正有负

Tip2: assign suitable credit

解决：同一场游戏里，所有的action都有一样的weight

(理想情况下sample足够多次可以解决该问题)

R-->从t开始到结束的所有reward，再对比较未来的reward做discount on

（b can be state-dependent, later）

*Advantage Function*: How good it is if we take At other than other Attions at St. Estimated by "critic"(later)











