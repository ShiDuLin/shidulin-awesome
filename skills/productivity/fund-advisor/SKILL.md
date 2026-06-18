---
name: fund-advisor
description: "基金定投顾问。定投计算（复利+真实年化）、收益模拟、资产配置、再平衡建议、止盈策略、基金类型科普。"
---

# fund-advisor

## 核心能力

1. **定投收益计算** - 计算每月定投的复利收益、真实年化收益率
2. **多收益率对比** - 对比不同年化收益率下的定投结果
3. **资产配置建议** - 根据风险偏好（保守/稳健/激进）给出配置方案
4. **投资组合再平衡** - 分析当前持仓偏离度，给出调整建议
5. **风险评估工具** - 夏普比率、最大回撤、VaR、蒙特卡罗模拟
6. **财务规划** - FIRE财务自由计算、IRR内部收益率、持仓成本分析

## 使用方式

用户可以询问以下类型的问题：

- "每月定投2000元，年化8%，定投10年能赚多少？"
- "帮我做一个10万元的稳健型资产配置"
- "对比一下5%、8%、12%收益率的定投效果"
- "我的持仓是股票5万、债券3万、货币2万，需要调整吗？"
- "基金有哪些类型？"
- "稳健型投资者应该怎么定投？"
- "帮我算一下夏普比率，年化收益15%，波动率20%，无风险利率3%"
- "我想FIRE，年支出12万，投资收益6%，需要多少钱？"

## Commands

| Command | Usage | Description |
|---------|-------|-------------|
| `invest` | `python3 scripts/fund.py invest "月定投额" "年化收益%" "定投年数"` | 定投收益计算 |
| `dca` | `python3 scripts/fund.py dca "月定投额" "年化收益%" "定投年数"` | 定投计算器（同invest，含复利+真实年化） |
| `compare` | `python3 scripts/fund.py compare "金额" "年数" "收益率1%,收益率2%,收益率3%"` | 多收益率对比 |
| `allocate` | `python3 scripts/fund.py allocate "保守\|稳健\|激进" "总金额"` | 资产配置建议（三种方案详细配置+金额） |
| `rebalance` | `python3 scripts/fund.py rebalance "股票50000,债券30000,货币20000"` | 再平衡建议（偏离目标配置时提醒调整） |
| `types` | `python3 scripts/fund.py types` | 基金类型科普 |
| `strategy` | `python3 scripts/fund.py strategy "风险偏好"` | 定投策略建议（保守/稳健/积极） |
| `sharpe` | `python3 scripts/fund.py sharpe "年化收益%" "年化波动率%" "无风险利率%"` | 夏普比率计算 |
| `maxdd` | `python3 scripts/fund.py maxdd "净值序列,逗号分隔"` | 最大回撤分析 |
| `kelly` | `python3 scripts/fund.py kelly "胜率%" "赔率"` | 凯利公式仓位计算 |
| `monte` | `python3 scripts/fund.py monte "月定投额" "年化收益%" "年化波动率%" "年数"` | 蒙特卡罗模拟 |
| `fire` | `python3 scripts/fund.py fire "年支出" "年投资收益%" "当前存款"` | FIRE财务自由计算 |
| `var` | `python3 scripts/fund.py var "投资总额" "年化收益%" "年化波动率%" "置信度%"` | VaR风险价值 |
| `irr` | `python3 scripts/fund.py irr "现金流序列,逗号分隔"` | 内部收益率计算 |
| `cost` | `python3 scripts/fund.py cost "买入记录:价格x份额,价格x份额,..."` | 持仓成本分析 |
| `help` | `python3 scripts/fund.py help` | 显示帮助信息 |

## Examples

```bash
# 每月定投2000元，年化8%，定投10年
python3 scripts/fund.py invest 2000 8 10

# 定投计算器（同invest）
python3 scripts/fund.py dca 3000 10 20

# 月投1000，10年，对比5%/8%/12%
python3 scripts/fund.py compare 1000 10 5,8,12

# 10万元稳健型资产配置
python3 scripts/fund.py allocate 稳健 100000

# 持仓再平衡分析
python3 scripts/fund.py rebalance "股票50000,债券30000,货币20000"

# 查看基金类型介绍
python3 scripts/fund.py types

# 获取稳健型策略建议
python3 scripts/fund.py strategy 稳健

# 计算夏普比率
python3 scripts/fund.py sharpe 15 20 3

# FIRE计算
python3 scripts/fund.py fire 120000 6 500000

# 蒙特卡罗模拟
python3 scripts/fund.py monte 1000 10 15 20

# 持仓成本分析
python3 scripts/fund.py cost 1.2x1000,1.0x2000,0.8x3000
```

## Reference

- 参考文档: `tips.md` — 基金投资实用指南（定投策略、资产配置、避坑指南）

## Notes

- 收益为理论模拟，不代表实际投资收益
- 纯本地计算，无需联网
- Python 3.6+ 兼容
- 基金有风险，投资需谨慎
