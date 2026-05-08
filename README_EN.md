<p align="center">
  <a href="./README.md">🇨🇳 简体中文</a> · <b>🇺🇸 English</b>
</p>

<p align="center">
  <img src="./assets/logo.png" alt="Doforu Logo" width="120"/>
</p>

<h1 align="center" style="border-bottom: none;">Doforu</h1>

<p align="center">
  <strong>One sentence to orchestrate multi-Agent execution</strong><br/>
  Just describe what you need — Doforu instantly breaks it down and dispatches multiple Agents in parallel.<br/>
  Coding, analysis, writing — get the full deliverable in one shot.
</p>

<p align="center">
  <a href="https://doforu.app/en"><img src="https://img.shields.io/badge/Website-Download-blue.svg" alt="Download"></a>
  <img src="https://img.shields.io/badge/version-3.5.0-blue.svg" alt="Version">
  <img src="https://img.shields.io/badge/macOS-Supported-000000?logo=apple&logoColor=white" alt="macOS">
  <img src="https://img.shields.io/badge/Windows-Supported-0078D6?logo=windows&logoColor=white" alt="Windows">
</p>

<p align="center">
  <b>First Release</b> · 
  <b>Custom Skills</b> · 
  <b>100%</b> Local Privacy · 
  <b>Bring Your Own API Key</b>
</p>

> 💡 **This repository is the official documentation and community feedback hub for Doforu.** Doforu is a closed-source commercial product; its source code is not publicly available. Please submit feedback and feature requests via [Issues](https://github.com/yctech2026/Doforu-APP/issues).

## Core Concept

**You say one sentence → Doforu breaks down the task → Multiple Agents execute in parallel → Delivers complete results**

No prompt engineering. No tool switching. The main Agent dynamically assembles sub-Agents to work simultaneously — automatically dividing labor, collaborating, and delivering.

> **[Watch Demo](https://doforu.app/demo)**

<p align="center">
  <img src="./assets/screenshot.png" alt="Doforu Main Interface" width="720"/>
</p>

## Use Cases

| Role | Typical Scenario | Example Prompt | Doforu Delivers |
|------|-----------------|---------------|----------------|
| **Developer** | Full-stack development, auto-fix, refactoring, tests | "Build a to-do app with login, React + TS, dark mode support." | A complete project ready to `npm run dev` |
| **Product Manager** | PRD writing, data analysis, interactive prototypes | "Analyze last quarter's retention data and output a report with charts." | Cleaned CSV + visualizations + analysis report |
| **Ops / Analyst** | Data cleaning, visualization, copywriting at scale | "Write 5 warm and healing Xiaohongshu (Red) posts with emojis." | 5 ready-to-publish posts + alternative headlines |
| **Indie Founder** | From idea to demo-ready MVP | "Build a landing page for our SaaS product with pricing and team sections." | A deployable static site + copy |

> Behind every run: The main Agent auto-evaluates complexity → lightweight tasks go to `fast` SubAgents, deep tasks go to `extreme` SubAgents → multiple SubAgents execute in parallel in the same round → auto-correction and aggregated delivery.

## Core Capabilities

- **Orchestrator Intelligent Dispatch** — Receives your instruction, understands intent, evaluates complexity, breaks tasks into parallel subtasks, and dynamically assigns them to the most suitable sub-Agents
- **Plan Instant Planning** — Analyzes your requirements and outputs a complete execution blueprint (steps, tool selection, estimated time). Confirm manually, then switch to Agent or Orchestrator mode to run
- **Agent Parallel Execution** — Multiple sub-Agents work simultaneously, each responsible for their part, automatically correcting errors, collaborating, and aggregating results into a complete deliverable
- **Evolving Skills** — Create or refine custom Skills in one sentence. Teach it once, reuse forever. The more your team uses it, the better it understands you
- **MCP Ecosystem Integration** — Seamlessly connects with databases, Figma, Slack, GitHub, and other external tools
- **Desktop-Native Experience** — Direct read/write to the local file system, deeply integrated with your development environment

## Product Comparison

| Capability | Cursor | Claude Code | Doforu |
|------------|--------|-------------|--------|
| Product Form | AI coding IDE (VS Code fork) | Terminal CLI coding Agent | **Desktop Agent Orchestrator** |
| Complex Tasks | Agent mode step-by-step | Single-thread terminal interaction | **One sentence, multi-Agent parallel delivery** |
| Auto Execution | Code editing + terminal | File I/O + command execution | **Auto write files, run, fix, generate reports** |
| Custom Workflow | Relies on `.cursorrules` config | Adjusted via conversation context | **Natural language-defined Skills, permanently reusable** |
| Model Support | Proprietary (GPT/Claude etc.) | Claude only | **15+ domestic & international models + local models** |
| Billing | Per Premium Request (~1.6/day Free) | Per API token consumption | **Platform fee only; API costs billed directly by providers** |
| Non-Developer Friendly | Developer-oriented | Developer-oriented | **One sentence, anyone can use** |

## Installation & Launch

### System Requirements

| OS | Minimum Version | Architecture | Recommended |
|----|-----------------|--------------|-------------|
| macOS | 12 (Monterey)+ | Apple Silicon / Intel | 8 GB RAM, 2 GB disk space |
| Windows | Windows 10+ | x64 / ARM64 | 8 GB RAM, 2 GB disk space |

### Download & Install

**Method 1: Official Website (Recommended)**

1. Visit [doforu.app/en](https://doforu.app/en)
2. Click "Download Now" and select your system version
3. Install and launch the app

**Method 2: GitHub Releases**

1. Go to the [Releases page](https://github.com/yctech2026/Doforu-APP/releases)
2. Download the latest package:
   - macOS: `Doforu-3.5.0-universal.dmg`
   - Windows: `Doforu-3.5.0-x64.exe`
3. Run the installer

### First Launch

1. **macOS**: Open the `.dmg`, drag Doforu to Applications. On first launch, allow it in **System Settings → Privacy & Security**.
2. **Windows**: Run the installer, follow the wizard. When the firewall prompt appears, allow network access (used to connect directly to model provider APIs).
3. On first open, select your preferred model and enter your API Key, then follow the prompts to complete initial setup.

## Quick Start

After installation, describe your task in natural language in the main interface input box:

> "Build a to-do app with login, React + TypeScript, dark mode support."

### Step 1: Choose Execution Mode

Select the execution method based on your needs:

| Mode | Best For | Description |
|------|----------|-------------|
| **Plan** | Want to see the plan first | Analyzes requirements, outputs a complete execution blueprint (steps, tool selection, estimated time). Run after confirmation |
| **Agent** | Simple tasks, quick execution | Runs directly with a single Agent. Suitable for copywriting, code snippets, simple queries |
| **Orchestrator** | Complex tasks, multi-Agent collaboration | Main Agent auto-breaks down tasks, dispatches multiple sub-Agents in parallel. Best for full-stack development, refactoring, deep analysis, multi-file collaboration |

> 💡 Not sure which to pick? Just use **Orchestrator**. It auto-evaluates complexity: lightweight tasks go to `fast` SubAgents, deep tasks go to `extreme` SubAgents — no manual selection needed.

### Step 2: Monitor Execution

The conversation stream displays the full execution in real time:
- **AI Response Stream** — Outputs reasoning and results word by word
- **Tool Call Cards** — Each tool (read file, write code, execute command, call SubAgent, etc.) displayed as a card; click to view parameters and return values
- **Status Indicator** — Bottom status bar shows current mode (Agent / Plan / Orchestrator running...)
- **Interrupt Anytime** — Click the bottom "Stop" button to immediately terminate the current task

### Step 3: Review & Iterate

After task completion, results are fully presented in the conversation stream:
- **Output Summary** — AI automatically aggregates deliverables and key conclusions
- **File Changes** — File write/edit operations show line change summaries (+N −M)
- **Screenshot Save** — Hover over any AI response, click the bottom-right button to save that reply as a PNG
- **Keep Iterating** — Send new instructions directly in the bottom input box to refine based on current context or start a new task

**Try it now 👉 [doforu.app/en](https://doforu.app/en)**

## Plans & Pricing

| Capability | Free | Pro |
|------------|------|-----|
| **Complete Task Runs** | **15 / day** | **300 / day** |
| Plan Mode (Task Planning) | ✓ | ✓ |
| Custom Skills | ✓ | Unlimited |
| Long-term Memory | — | ✓ |
| MCP Connections | 1 | Unlimited |
| Context Compression | Delayed trigger | Proactive optimization |

Pro pricing: [doforu.app/pricing](https://doforu.app/pricing)

## System & Models

**Supported OS**: macOS 12+ · Windows 10+

**Supported Models**:

- **International**: OpenAI (GPT-5.5, GPT-5.4, o3) · Anthropic (Claude Opus 4.7, Claude Sonnet 4.5) · Google (Gemini 3.1) · DeepSeek (DeepSeek V4)
- **China**: Alibaba Qwen (Qwen 3.6) · ByteDance Doubao · Moonshot Kimi · Baidu ERNIE (ERNIE 5.0) · Zhipu GLM · iFlytek Spark · Baichuan · SenseTime senseChat
- **Local**: OpenAI API-compatible local models (Ollama, vLLM, etc.)

**Privacy & Cost**: 100% local execution. API Key stays in your hands, connects directly to providers. Doforu only charges for complete task runs on the client platform; API call costs go directly to the providers — Doforu does not intermediate, markup, or profit from API usage.

## Get Help

- [Documentation](https://doforu.app/docs) — Self-service
- [GitHub Issues](https://github.com/yctech2026/Doforu-APP/issues) — Bug reports & feature requests
- WeCom / DingTalk — Enterprise support within 4 hours

[Create Issue](https://github.com/yctech2026/Doforu-APP/issues) · [Changelog](https://doforu.app/changelog)

## FAQ

### How many runs per day on the Free plan?

**15 complete task runs / day** — One run = a complete workflow from requirement to delivery.

| What you can do daily | Equivalent to |
|----------------------|---------------|
| Write **3–5** complete frontend pages | Includes requirement analysis + component selection + code + styling + self-testing |
| Generate **5–8** utility scripts | Includes logic design + edge cases + error handling + usage docs |
| Produce **2–3** data analysis reports | Includes data cleaning + visualizations + insight summary |
| Complete **3–5** technical research topics | Includes information search + multi-source comparison + solution evaluation |

### What's on Doforu's roadmap?

- **2026.04 — Multi-Agent Parallel Orchestration (Released)**  
  Orchestrator pure-coordinator mode is live, supporting `fast`/`extreme` dual-type SubAgent parallel execution with SSE real-time progress streaming.

- **2026.06 — Pro Plan Official Launch**  
  Quota management and machine-code licensing infrastructure are ready. Pro will unlock higher daily quotas, unlimited Skills, and proactive context compression.

- **2026.Q3 — Team Workspaces & Shared Skills**  
  Skills already support local directory management and Claude Code-compatible formats. The Team plan will open workspace collaboration and Skills sharing.

## Enterprise

Enterprise teams are welcome to inquire about procurement and custom partnerships. Please email **alex@yichaotech.com.cn** — we will respond within 1 business day.

## License

This software is closed-source commercial software. Copyright belongs to Doforu. All rights reserved. Unauthorized decompilation, reverse engineering, distribution, or derivative development is prohibited.

© 2026 Doforu. All rights reserved.
