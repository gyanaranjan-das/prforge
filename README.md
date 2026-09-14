<div align="center">
  <h1>🛠️ prforge</h1>
  <p><strong>The Autonomous GitHub Developer Agent</strong></p>
  <p>
    <a href="https://github.com/gyanaranjan-das/prforge/issues">Issues</a>
    ·
    <a href="https://github.com/gyanaranjan-das/prforge/pulls">Pull Requests</a>
    ·
    <a href="#license">License</a>
  </p>
</div>

---

## 📖 Overview

**prforge** (pronounced "pull-request forge") is an autonomous, AI-powered developer agent. Point it at a GitHub repository and an issue, and it will:
1. **Explore** the codebase to understand the context.
2. **Plan** out the required changes.
3. **Implement** the fix or feature.
4. **Verify** by running your test suite in a sandbox.
5. **Deliver** a polished, draft Pull Request ready for human review.

Instead of manually guiding the AI through every file and edit, `prforge` operates end-to-end like a junior-to-mid level developer on your team.

## ✨ Features (v1 Scope)

- **Issue-Driven**: Triggered via a GitHub issue or CLI command.
- **Smart Exploration**: Locates relevant files via intelligent search and AST/symbol parsing, going beyond simple `grep`.
- **Pre-execution Planning**: Proposes an edit plan before touching any code to ensure accuracy.
- **Self-Healing Verification**: Runs the repository's test suite, parses failures, and automatically fixes mistakes.
- **Human-in-the-Loop**: Outputs a **draft PR** for final human review.

*(Note: Fully autonomous merges and multi-tenant hosted services are currently out of scope for v1. `prforge` operates as a local CLI tool or a GitHub Action).*

## 🏗️ Architecture & Layout

The project is structured to separate the agent's core brain from its configuration and testing suites.

- `src/` — The agent core: explore, plan, edit, verify, and PR generation modules.
- `tests/` — Test suites ensuring `prforge` operates reliably.
- `config/` — Repository configuration, prompt templates, and tool settings.

## 🚀 Getting Started

*(Initialization instructions coming soon as the core CLI is developed.)*

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/gyanaranjan-das/prforge/issues). 
As we build out the v1 milestone, please open an issue to discuss any major changes before submitting a PR.

## 📄 License

This project is [MIT licensed](./LICENSE).
