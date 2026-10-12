# AZEN

Building at the intersection of AI agent infrastructure, verifiable reasoning systems, and onchain finance.

## Projects

### [RepoPilot](https://github.com/azen07508-debug/repopilot)

The quality layer for agents that ship code. Point it at a public repo and get
evidence-backed findings (every claim carries a `path:line:reason` pointer) and
rule-based reproducible scoring — plus a **fix plan per finding**: ordered steps,
tests to add, acceptance criteria, and an `agentInstructions` block you can hand
straight to Codex or Claude Code.

Re-audit and see what actually changed: score movement attributed rule by rule,
findings split into resolved / new / still-open. The loop is
audit → fix plan → fix → re-audit → compare, over HTTP or MCP.

Static analysis only — it never executes the audited repository's code.

`TypeScript` `Fastify` `MCP` `x402`

### [MingLi Agent (agent-knowledge-os)](https://github.com/azen07508-debug/agent-knowledge-os)

Verifiable Chinese astrology reasoning system. Separates deterministic chart
computation from multi-agent reasoning, using a rule engine for classical texts
and an **Evidence Layer** to trace every conclusion back to classical sources
without LLM hallucinations. Evaluated continuously against MingLi-Bench and fate-bench.

`Python` `Multi-Agent` `Evidence Layer` `Rule Engine` `Deterministic Computing`

### [XGuard Hook](https://github.com/azen07508-debug/xguard-hook)

Dynamic risk-fee [Uniswap v4](https://docs.uniswap.org/contracts/v4/overview) Hook for new-asset,
meme, and low-cap pools on X Layer. LP fees scale with swap impact — `Normal` 0.30%,
`Warning` 1.00%, `Protected` 3.00% — and the pool's risk state is verifiable onchain, so
traders and LPs price the same risk the contract does.

Ships with a demo router, a live frontend, and a Foundry test suite covering the fee
override, risk decay, and hard-threshold blocking paths.

`Solidity` `Foundry` `Uniswap v4` `X Layer` — [live demo](https://xguard-hook.vercel.app)

## Focus

- **AI Agent Infrastructure & DevTools** — release quality gates, audit-fix loops, MCP tooling
- **Verifiable AI & Reasoning Systems** — evidence layers, rule engines, deterministic execution
- **DeFi Primitives** — Uniswap v4 Hooks, onchain dynamic risk pricing, X Layer

---

_中文：深耕 AI Agent 基础设施、可验证推理系统与链上金融的交叉领域。_
- _**RepoPilot**：面向代码生成 Agent 的发布把关层与审计修复闭环（HTTP / MCP 静态分析）；_
- _**MingLi Agent**：融合确定性排盘、典籍规则引擎与证据链追踪的可验证命理推理智能体；_
- _**XGuard Hook**：部署于 X Layer 的 Uniswap v4 动态风险费率 Hook。_
