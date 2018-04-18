# minority game in 50 lines

## 关于[minority game](https://en.wikipedia.org/wiki/El_Farol_Bar_problem#Minority_game)

N个主体进行静态演化博弈，每个主体被随机赋予s个策略。
在每个周期，每个主体根据最近m个历史获胜信息，选择自身最佳策略，做出选择：
- 0(在家)，或者
- 1(酒吧)。

然后根据所有主体的选择情况作出胜负判断：
- 选择少数者的主体获胜，其所用策略积分+1，
- 选择多数者的主体失败，其所用策略积分-1(传统MG规则)。

如此，当前局面被清除，并进入下一周期。
