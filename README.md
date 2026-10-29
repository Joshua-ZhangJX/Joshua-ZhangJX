# Jiaxuan (Joshua) Zhang

Incoming M.S. in Computer Science (Artificial Intelligence), University of Southern California — Spring 2027 ·
B.Eng. in Artificial Intelligence, South China Normal University

I build LLM agent harnesses and study what makes them dependable — evaluating them against ground truth,
and watching how context and memory behave as traces grow. Most of this work lives in private repositories;
what I can point to is below, and I am glad to walk through the rest.

## What I work on

- **Capability runtimes** — retrieval and browser runtimes behind a stable tool registry, so the model's tool
  vocabulary stays put when the provider underneath changes.
- **Control and permissions** — session-scoped permissions, a bound on agent loop rounds, and risk-gated
  approval, each covered by unit tests.
- **Evaluation** — fixture-driven end-to-end tests, fault injection, and acceptance runs reconciled against
  raw exports. I try to state what a run does *not* establish.

## Selected work

**Archer — agent harness for industrial analytics** · `Go` `TypeScript` `SQLite` · *private repository*

- Built the `web_search` retrieval runtime: Bing HTML backend, captcha and redirect handling, structured
  citations, table-driven fixture tests.
- Added browser automation as a first-class capability — 12 interaction tools behind a table-driven CLI
  mapping, with fixture-driven end-to-end tests.
- Implemented session-scoped permissions, a max-rounds bound on the agent loop, and risk-gated
  auto-approval, with Go unit tests.

**Attribution agent over a Power BI semantic model** · `Python` `DAX` · *private repository*

- Owned the design and validation of an agent that answers business questions over a semantic model and
  produces auditable reports: parameterized DAX catalog, immutable result store, evidence citations,
  multi-turn recovery across service restarts.
- Defined the acceptance protocol — 10 rounds with a real model, every number reconciled against 57,938
  rows of raw export (3,965 checks, zero diff). Fault injection surfaced two conversation-compaction
  defects; both were fixed and re-verified.

**Time-series foundation models for demand forecasting** · `Python` `TimesFM` `MCP`

- Zero-shot retail demand forecasting with TimesFM 3.0, wrapped as an MCP server so an agent can call the
  forecaster as a tool.

## Publication

**Research on AGV Path Planning in Automated Warehouses** — ICBSEMCT 2026 (accepted).
Turn-penalty A*: **−52.3% turns** versus standard A* in simulation.

## Contact

zhangj50@usc.edu · Shenzhen, China

<sub>Last updated: 2026-10</sub>
