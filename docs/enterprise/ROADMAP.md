# Grok Enterprise AI Workstation Roadmap

## Product objective

Transform the synced Grok Build codebase into an independently valuable enterprise AI workstation while preserving a low-conflict path for future upstream imports.

The upstream tree remains the execution engine and terminal experience. Enterprise functionality lives in an isolated workspace under `enterprise/` and integrates through stable adapters, process boundaries, ACP, MCP, hooks, configuration and explicitly maintained bridge crates.

## Product identity

Working product name: **RedZen Enterprise AI Workstation**.

The product is not a renamed Grok CLI. It is an enterprise control plane that coordinates models, agents, tools, policies, memory, users and audit data while using Grok Build as one execution client.

## Non-negotiable architecture principles

1. Do not edit the generated root Cargo workspace for enterprise membership.
2. Keep upstream code replaceable and periodically synchronizable.
3. Put enterprise business