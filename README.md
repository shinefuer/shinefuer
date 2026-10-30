<div align="center">

![Wu Manruo — 高性能 × 成本效率的 Coding Agent 框架](assets/header.svg)

![coding agent runtime](https://img.shields.io/badge/focus-coding_agent_runtime-059669?style=flat-square)
![cost efficiency](https://img.shields.io/badge/focus-cost_efficiency-b45309?style=flat-square)
![offline-first](https://img.shields.io/badge/offline--first-planted_optima-5c6b85?style=flat-square)

</div>

![研究旅程：frugent](assets/journey.svg)

## 项目

| 项目 | 研究方向 | 已实现内容 |
|---|---|---|
| [frugent](https://github.com/shinefuer/frugent) | 成本效率 Coding Agent 运行时 | 版本化上下文存储与前缀树 token 核算、前缀感知 prompt-cache 路由（小迹上可证近优）、投毒安全语义缓存（MinHash/shingle 模糊键 + 等价性质测试）、token 预算上下文压缩（knapsack 精确解 + needle-recall 实测降级曲线）、请求批处理/去重（single-flight 订阅者结果等价）、级联模型路由（质量门升级 + 合成难度混合上恢复 DP 最优）、硬预算调度（随机化性质套件证明永不超支 + 降级阶梯）、span 级成本归因（守恒性质 + trace diff）、allowlist 沙箱工具执行器（路径穿越/注入拒绝性质）、合成编码负载工厂（植入最优成本画像）、离线基准与确定性 SVG/HTML 成本报告、完整 CLI |

<div align="center">

[![CI](https://github.com/shinefuer/frugent/actions/workflows/ci.yml/badge.svg)](https://github.com/shinefuer/frugent/actions/workflows/ci.yml)
[![Release](https://img.shields.io/github/v/release/shinefuer/frugent?style=flat-square&color=fbbf24)](https://github.com/shinefuer/frugent/releases)
![commits](https://img.shields.io/badge/commits-523-34d399?style=flat-square)
![tests](https://img.shields.io/badge/tests-1280_passed-a78bfa?style=flat-square)

</div>

523 次提交（2025.01 — 2026.10）· 33 个源码模块 · 4 个可运行离线示例 · 每次提交都经过构建、测试与格式检查。所有测量数字来自带植入最优解的确定性合成负载与虚构费率卡：无真实模型端点、无预训练权重、全离线可复现。

## 技术栈

![Python](https://img.shields.io/badge/Python-3.11%2B-3776ab?style=flat-square&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-core-013243?style=flat-square&logo=numpy&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-CPU_extra-ee4c2c?style=flat-square&logo=pytorch&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-property_%2B_golden-0a9edc?style=flat-square)
![ruff](https://img.shields.io/badge/ruff-format_%2B_lint-d7ff64?style=flat-square)
![GitHub Actions](https://img.shields.io/badge/CI-3.11_%2F_3.12_%2F_3.13-2088ff?style=flat-square&logo=githubactions&logoColor=white)

## 活动

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/shinefuer/shinefuer/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/shinefuer/shinefuer/output/github-snake.svg" />
  <img alt="contribution snake" src="https://raw.githubusercontent.com/shinefuer/shinefuer/output/github-snake.svg" />
</picture>

## 当前关注

- 前缀感知缓存路由的经济学：命中率、TTL 与驱逐策略在合成迹上的近优性边界。
- 级联质量门的校准：置信度阈值、验证器成本与 DP 最优梯度的差距收敛。
- 成本归因方法学：span 守恒性质、缓存节省与批处理折扣的逐任务分解。
