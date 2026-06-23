<img width="4400" height="657" alt="Designer (5)" src="https://github.com/user-attachments/assets/a51d37d9-4a4a-4fd4-ac30-547a2d23f278" />

# GitHub Copilot Advanced Labs — The Agentic SDLC

A hands-on workshop that progressively builds **Agentic SDLC** skills. Across 8 labs (~1 hour each), participants go from using Copilot as a suggestion tool to orchestrating a fully autonomous development pipeline.

---

## The Progression

```
Lab 01-03:  Copilot as a TOOL         → you do the work, Copilot helps
Lab 04-05:  Copilot as a TEAM MEMBER  → you set standards, Copilot follows
Lab 06-07:  Copilot as a DEVELOPER    → you approve, Copilot does the work
Lab 08:     Copilot as a PIPELINE     → the loop runs itself
```

---

## Labs

| # | Lab | SDLC Phase | Autonomy | Folder |
|---|-----|-----------|----------|--------|
| 01 | [Code Generation Fundamentals](lab01/) | Code | 🟢 Human writes, Copilot suggests | `lab01/` |
| 02 | [Testing with Copilot](lab02/) | Test | 🟢 Human directs, Copilot generates | `lab02/` |
| 03 | [Debugging & Troubleshooting](lab03/) | Debug | 🟡 Human points, Copilot fixes | `lab03/` |
| 04 | [Context Engineering](lab04/) | Cross-cutting | 🟡 Human configures, Copilot follows | `lab04/` |
| 05 | [RPI Workflow: GitHub MCP, HVE & Coding Agent](lab05/) | Review | 🟠 Human asks, Agent researches | `lab05/` |
| 06 | [MCP Expansion for Your SDLC](lab06/) | Code+Test+Debug | 🔴 Human approves, Agent implements | `lab06/` |
| 07 | [Release Workflow and Infrastructure as Code](lab07/) | Integration → Deployment → Release | 🟡 Human reviews, Copilot automates | `lab07/` |
| 08 | [Capstone: Task Board from Spec to Cloud](lab08/) | Spec → Test → Build → Deploy | 🔴🔴 Agent runs end-to-end | `lab08/` |

---

## Prerequisites

- **GitHub Copilot** license (Individual, Business, or Enterprise)
- **VS Code** with the GitHub Copilot and GitHub Copilot Chat extensions
- **Python 3.10+**
- **GitHub CLI** (`gh`) with the Copilot extension — `gh extension install github/gh-copilot`
- **[HVE Core](https://github.com/microsoft/hve-core)** VS Code extension (Labs 04–08) — install from the [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=ise-hve-essentials.hve-core)
- Basic familiarity with Git and GitHub

---

## Getting Started

```bash
git clone https://github.com/martaldsantos/ghcp-labs.git
cd ghcp-labs
```

Then navigate to the lab folder and follow its README:

```bash
cd lab01
```

---

## Course Structure

Each lab follows a consistent format:

1. **Scaffolded project** — realistic production code is provided
2. **Starter skeletons** — partially completed files with TODOs for participants
3. **Step-by-step instructions** — timed parts with clear objectives
4. **Hints** — expandable hints for when participants get stuck
5. **Solutions** — reference implementations in a `solutions/` folder (where applicable)

---

## Lab 08: Capstone Overview

**Lab 08** brings everything together in a practical greenfield capstone. Participants build a fully functional kanban Task Board app (~2 hours) that goes from a one-page PRD to live Azure deployment:

- **Spec Refinement** — Write your PRD and have agents transform it into testable FRDs with acceptance criteria
- **UI/UX Design** — Generate and iterate on interactive wireframes
- **Test Scaffolding** — Derive comprehensive tests directly from Gherkin scenarios
- **Implementation** — Agents build backend (Express) and frontend (Next.js) to make tests pass
- **Deployment** — Provision Azure infrastructure and run smoke tests against the live app

No production code is written by you—only the spec. The spec drives all tests, implementation, and deployment verification. This mirrors the [spec2cloud Microhack](https://github.com/EmeaAppGbb/spec2cloud-microhack-greenfield) approach.
