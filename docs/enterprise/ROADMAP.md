# Grok Enterprise AI Workstation Roadmap

## Product objective

Transform the synced Grok Build codebase into an independently valuable enterprise AI workstation while preserving a low-conflict path for future upstream imports.

The upstream tree remains the execution engine and terminal experience. Enterprise functionality lives in an isolated workspace under `enterprise/` and integrates through stable adapters, process boundaries, ACP, MCP, hooks, configuration and explicitly maintained bridge