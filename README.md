<div align="center">

# 🤖 Awesome AI Coding Agent Tools

**Tools, libraries, MCP servers, and frameworks that power AI coding agents.**

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Lint](https://github.com/namphuongtran/awesome-ai-coding-agent-tools/actions/workflows/lint.yml/badge.svg)](https://github.com/namphuongtran/awesome-ai-coding-agent-tools/actions/workflows/lint.yml)
[![Links](https://github.com/namphuongtran/awesome-ai-coding-agent-tools/actions/workflows/links.yml/badge.svg)](https://github.com/namphuongtran/awesome-ai-coding-agent-tools/actions/workflows/links.yml)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](../../pulls)
![Tools](https://img.shields.io/badge/tools-132-blue.svg)
![Categories](https://img.shields.io/badge/categories-27-purple.svg)
![Made with](https://img.shields.io/badge/made%20with-%E2%9D%A4-red.svg)

---

**✨ Featured Tools**

<p>
  <a href="https://github.com/modelcontextprotocol/servers"><img src="https://img.shields.io/github/stars/modelcontextprotocol/servers?style=for-the-badge&logo=github&logoColor=white&label=MCP%20Servers&color=0080FF" alt="MCP Servers" /></a>
  <a href="https://github.com/anthropics/skills"><img src="https://img.shields.io/github/stars/anthropics/skills?style=for-the-badge&logo=anthropic&logoColor=white&label=Anthropic%20Skills&color=D4A574" alt="Anthropic Skills" /></a>
  <a href="https://github.com/langchain-ai/langchain"><img src="https://img.shields.io/github/stars/langchain-ai/langchain?style=for-the-badge&logo=langchain&logoColor=white&label=LangChain&color=1C3A3A" alt="LangChain" /></a>
  <a href="https://github.com/langchain-ai/langgraph"><img src="https://img.shields.io/github/stars/langchain-ai/langgraph?style=for-the-badge&logo=langchain&logoColor=white&label=LangGraph&color=00C896" alt="LangGraph" /></a>
</p>
<p>
  <a href="https://github.com/vercel/ai"><img src="https://img.shields.io/github/stars/vercel/ai?style=for-the-badge&logo=vercel&logoColor=white&label=Vercel%20AI&color=000000" alt="Vercel AI SDK" /></a>
  <a href="https://github.com/e2b-dev/E2B"><img src="https://img.shields.io/github/stars/e2b-dev/E2B?style=for-the-badge&logo=python&logoColor=white&label=E2B&color=FF6B35" alt="E2B" /></a>
  <a href="https://github.com/langfuse/langfuse"><img src="https://img.shields.io/github/stars/langfuse/langfuse?style=for-the-badge&logo=github&logoColor=white&label=Langfuse&color=6F42C1" alt="Langfuse" /></a>
  <a href="https://github.com/yamadashy/repomix"><img src="https://img.shields.io/github/stars/yamadashy/repomix?style=for-the-badge&logo=github&logoColor=white&label=Repomix&color=0066CC" alt="Repomix" /></a>
</p>

</div>

---

This list collects the **tools, libraries, MCP servers, and frameworks that power AI coding agents** — from the skills and plugins that extend them, to the SDKs you'd build them with, to the supporting layers (memory, sandboxing, evals, observability, benchmarks) that turn demos into production. The agents themselves (Claude Code, Cursor, aider, Cline, …) live in their own repos; this list is the ecosystem around them. Inclusion is based on visible community use rather than star counts. Every entry includes nested **Strengths** and **Caveats** bullets so you can compare at a glance.

## Contents

- [Extensions, Skills & Rules](#extensions-skills--rules)
  - [Claude Code Skills & Plugins](#claude-code-skills--plugins)
  - [Cursor Rules](#cursor-rules)
  - [MCP Servers](#mcp-servers)
  - [Curated Awesome Lists](#curated-awesome-lists)
  - [Methodologies & Spec-Driven Workflows](#methodologies--spec-driven-workflows)
  - [Skill & Plugin Marketplaces](#skill--plugin-marketplaces)
- [Agent SDKs & Frameworks](#agent-sdks--frameworks)
  - [Official Vendor SDKs](#official-vendor-sdks)
  - [Orchestration Frameworks](#orchestration-frameworks)
  - [Lightweight & Typed](#lightweight--typed)
  - [Structured Output & Multi-Provider](#structured-output--multi-provider)
  - [Stateful Agents](#stateful-agents)
- [Supporting Infrastructure](#supporting-infrastructure)
  - [Memory](#memory)
  - [Vector Databases](#vector-databases)
  - [Codebase Context](#codebase-context)
  - [Sandboxing & Execution](#sandboxing--execution)
  - [Workflow & Pipeline Orchestration](#workflow--pipeline-orchestration)
  - [Evaluation](#evaluation)
  - [Observability](#observability)
  - [Prompt Management](#prompt-management)
  - [Benchmarks & Leaderboards](#benchmarks--leaderboards)
  - [Test Generation](#test-generation)
  - [Local LLM Runners](#local-llm-runners)
- [Learning Resources](#learning-resources)
  - [Articles & Blogs](#articles--blogs)
  - [Tutorials & Courses](#tutorials--courses)
  - [Books](#books)
  - [Podcasts](#podcasts)
  - [Datasets](#datasets)
- [Community](#community)

## Extensions, Skills & Rules

Add-ons that extend AI coding agents with new capabilities, knowledge, or rules.

### Claude Code Skills & Plugins

- [Anthropic Claude Cookbooks](https://github.com/anthropics/claude-cookbooks) - Notebooks and recipes for Claude skills, patterns, tool use, and memory management.
  - **Strengths:** 95+ Python Jupyter examples; RAG/classification/summarization; multimodal vision.
  - **Caveats:** Python-centric; assumes Claude API familiarity; rapid API changes.
- [Anthropic Claude Plugins Official](https://github.com/anthropics/claude-plugins-official) - Anthropic's official directory of curated Claude Code plugins.
  - **Strengths:** curated official plugins; simple install via CLI; standardized plugin structure.
  - **Caveats:** trust plugins before installing; limited quality control for external plugins; verify independently.
- [Anthropic Claude Quickstarts](https://github.com/anthropics/claude-quickstarts) - Deployable starter projects to jumpstart Claude API applications.
  - **Strengths:** ready-to-use templates; covers support/finance/automation/coding; well-documented.
  - **Caveats:** requires Claude API key; per-project setup; no production guarantees.
- [Anthropic Skills](https://github.com/anthropics/skills) - Official open standard repo for Agent Skills in `SKILL.md` format.
  - **Strengths:** simple folder-based structure; multi-platform (Code/AI/API); 131 production examples.
  - **Caveats:** educational/demo purpose; behavior variability vs documentation; testing required.
- [claude-mem](https://github.com/thedotmack/claude-mem) - Plugin that captures and injects session context for cross-session memory.
  - **Strengths:** ~10x token savings via 3-layer workflow; SQLite + FTS5 + Chroma retrieval; multi-IDE compatibility.
  - **Caveats:** requires Node.js 18+; lossy memory compression; vector-DB initialization overhead.
- [Everything Claude Code](https://github.com/affaan-m/ECC) - Performance-optimization system and tuning reference for the Claude Code agent harness.
  - **Strengths:** harness performance focus; benchmark-driven tuning; concise patterns.
  - **Caveats:** niche perf-focused audience; assumes Claude Code familiarity.
- [get-shit-done](https://github.com/gsd-build/get-shit-done) - Meta-prompting and context-engineering system for agent-distributed large projects.
  - **Strengths:** parallel isolated 200k-token contexts; persistent cross-session docs; auto-diagnose failures.
  - **Caveats:** sequential six-command workflow; best for large structured projects.
- [graphify](https://github.com/safishamsi/graphify) - Skill that turns code, docs, and media into navigable knowledge graphs.
  - **Strengths:** confidence tagging on relationships; god-node and surprising-connection detection; inline-comment rationale linking.
  - **Caveats:** local AST processing only; multimedia transcription via external APIs; first-run scales with project size.
- [gstack](https://github.com/garrytan/gstack) - Garry Tan's exact Claude Code setup with 23 opinionated role-based tools (CEO, Designer, Eng Manager, Release Manager, Doc Engineer, QA).
  - **Strengths:** role-based metaphor across the dev lifecycle; mirrors a production YC workflow; broad active community.
  - **Caveats:** highly opinionated about the specialist-team model; less flexible for unconventional workflows.
- [Karpathy-Inspired Claude Code Skills](https://github.com/multica-ai/andrej-karpathy-skills) - Compact Karpathy-style coding skills distilled into Claude Code-compatible format.
  - **Strengths:** Karpathy minimalism applied to skills; concise, pragmatic patterns; quick to adopt.
  - **Caveats:** personal interpretation; small skill count; opinionated style.
- [Matt Pocock's Skills](https://github.com/mattpocock/skills) - Personal Claude Code skill pack from Matt Pocock, drawn straight from his `.claude` directory.
  - **Strengths:** opinionated commands (`/grill-me`, `/write-a-prd`, `/tdd`, `/triage-issue`, `/git-guardrails`); failure-mode focus across planning/testing/safety; readable shell-based skills.
  - **Caveats:** small skill set; reflects one engineer's workflow; no built-in orchestration.
- [superpowers](https://github.com/obra/superpowers) - Agentic skills framework and methodology for Claude Code, Cursor, Codex, and Gemini CLI.
  - **Strengths:** TDD/RED-GREEN-REFACTOR built in; brainstorming + planning before code; Git-worktree mgmt for parallel work.
  - **Caveats:** philosophy-heavy; best results need cultural adoption.
- [Understand-Anything](https://github.com/Lum1104/Understand-Anything) - Interactive knowledge-graph explorer for codebases and documents.
  - **Strengths:** multi-view exploration (structural/business/semantic); guided onboarding tours; concurrent multi-agent pipeline.
  - **Caveats:** initial analysis pass needed; impact analysis is code-only, not runtime.

### Cursor Rules

- [awesome-cursor-rules-mdc](https://github.com/sanjeed5/awesome-cursor-rules-mdc) - Collection of Cursor `.mdc` rule files covering popular stacks.
  - **Strengths:** modern `.mdc` format; broad framework coverage; actively maintained.
  - **Caveats:** community contributions vary in depth; framework version drift.
- [awesome-cursorrules](https://github.com/PatrickJS/awesome-cursorrules) - Configuration files that customize Cursor's behavior per project.
  - **Strengths:** large catalog; primary community hub; widely linked from tutorials.
  - **Caveats:** older `.cursorrules` format alongside newer `.mdc`; rule quality varies.

### MCP Servers

- [awesome-mcp-servers (punkpeye)](https://github.com/punkpeye/awesome-mcp-servers) - Community catalog of Model Context Protocol servers.
  - **Strengths:** large index; sortable by category; community-driven additions.
  - **Caveats:** not curated for quality; dead links accumulate.
- [awesome-mcp-servers (wong2)](https://github.com/wong2/awesome-mcp-servers) - Curated list of Model Context Protocol servers.
  - **Strengths:** tighter curation; categorized; updated regularly.
  - **Caveats:** smaller than alternatives; subjective inclusion bar.
- [best-of-mcp-servers](https://github.com/tolkonepiu/best-of-mcp-servers) - Weekly-updated ranked list of MCP servers across the ecosystem.
  - **Strengths:** 400+ ranked MCP servers; quality scoring; weekly updates; transparent metrics.
  - **Caveats:** algorithmic ranking only; not a testing service; curation gaps.
- [C4 Model MCP](https://docs.structurizr.com/ai/mcp) - Structurizr's official MCP server for C4 architecture diagrams with DSL validation and PlantUML/Mermaid export.
  - **Strengths:** official C4 reference implementation; 23 MCP tools; Docker and Java 21 deployment.
  - **Caveats:** requires Java 21; experimental status; HTTP stateless mode limits some features.
- [Excalidraw MCP](https://github.com/excalidraw/excalidraw-mcp) - Official Excalidraw MCP server for streaming hand-drawn diagram creation from agents.
  - **Strengths:** official Excalidraw team implementation; mobile-optimized streaming UI; works with Claude/ChatGPT/VS Code/Goose.
  - **Caveats:** requires MCP-compatible client; local setup needs Node.js familiarity.
- [FastMCP](https://github.com/PrefectHQ/fastmcp) - Pythonic framework for building MCP servers and clients using decorators and type hints.
  - **Strengths:** decorator-based, type-hinted Python API; builds both servers and clients; broad community adoption (25k+ stars).
  - **Caveats:** Python-only; pre-1.0 breaking changes still possible.
- [Figma MCP](https://github.com/GLips/Figma-Context-MCP) - MCP server giving agents semantic access to Figma designs for design-to-code.
  - **Strengths:** agent access to Figma data; single-shot implementation; optimized for Cursor.
  - **Caveats:** requires Figma API token; configuration overhead; Cursor-focused; context filtering trade-off.
- [GitHub MCP Server](https://github.com/github/github-mcp-server) - GitHub's official MCP server giving agents access to repos, issues, pull requests, and Actions via the GitHub API.
  - **Strengths:** first-party from GitHub; covers repos, issues, PRs, Actions, and code search; widely adopted (30k+ stars).
  - **Caveats:** requires GitHub personal access token with appropriate scopes; rate-limited by token tier.
- [microsoft/mcp](https://github.com/microsoft/mcp) - Microsoft's official MCP server implementations.
  - **Strengths:** first-party Microsoft implementations; enterprise-aware; well-tested.
  - **Caveats:** Microsoft-stack bias; some servers are early.
- [modelcontextprotocol/inspector](https://github.com/modelcontextprotocol/inspector) - Official visual testing and debugging tool for MCP servers from the protocol working group.
  - **Strengths:** canonical MCP-server dev/test harness; interactive tool/resource exploration; first-party MCP working-group project.
  - **Caveats:** Node.js-based local CLI; intended for development, not production monitoring.
- [modelcontextprotocol/servers](https://github.com/modelcontextprotocol/servers) - Official MCP reference servers for filesystem, Git, GitHub, memory, and more.
  - **Strengths:** canonical reference; minimal dependencies; copy-pasteable for most agents.
  - **Caveats:** reference-quality, not production-hardened; security trade-offs are user responsibility.
- [Playwright MCP](https://github.com/microsoft/playwright-mcp) - Microsoft's MCP server for browser automation and end-to-end testing.
  - **Strengths:** accessibility tree (no vision models); fast and lightweight; avoids screenshot ambiguity.
  - **Caveats:** not a security boundary; headless Chromium only; profile conflicts under concurrency.
- [Serena](https://github.com/oraios/serena) - MCP toolkit giving agents IDE-like semantic retrieval and editing via Language Server Protocol.
  - **Strengths:** LSP-powered semantic ops (rename/references/navigation); multi-language; widely adopted (24k+ stars); free OSS.
  - **Caveats:** requires per-language LSP servers installed; setup complexity varies by language.
- [Stitch MCP](https://github.com/Kargatharaakash/stitch-mcp) - MCP bridge for Google Stitch AI UI design tool — extract design context and generate screens.
  - **Strengths:** zero-config after auth; cross-platform; instant access to design DNA (fonts/colors/layouts).
  - **Caveats:** requires Google Cloud credential setup; depends on Stitch platform availability.
- [Supabase MCP](https://github.com/supabase-community/supabase-mcp) - Connect Supabase databases to Claude Code, Cursor, and other LLMs.
  - **Strengths:** standardizes LLM↔Supabase interaction; comprehensive tooling; configurable security.
  - **Caveats:** pre-1.0 (breaking changes likely); limited self-hosted features; prompt injection possible.

### Curated Awesome Lists

- [awesome-agents](https://github.com/kyrolabs/awesome-agents) - Curated list of AI agents and frameworks.
  - **Strengths:** comprehensive directory; specialized use-case categorization; cutting-edge entries.
  - **Caveats:** no comparative analysis or selection guidance; maintenance uncertainty on listed projects.
- [awesome-ai-agents](https://github.com/jim-schwoebel/awesome_ai_agents) - Large index of resources and tools across the AI agents ecosystem.
  - **Strengths:** 1500+ resources; daily updates; multi-tier organization; community-driven.
  - **Caveats:** breadth over depth; rapid obsolescence risk; no quality vetting.
- [awesome-claude-code (hesreallyhim)](https://github.com/hesreallyhim/awesome-claude-code) - Skills, hooks, slash commands, agents, and plugins for Claude Code.
  - **Strengths:** quality and security emphasis; broad coverage of skills/hooks/commands.
  - **Caveats:** active restructuring underway; documentation in flux.
- [awesome-claude-code (jqueryscript)](https://github.com/jqueryscript/awesome-claude-code) - Curated tools, IDE integrations, and frameworks for Claude Code.
  - **Strengths:** 200+ tools catalogued; star-rating badges; operational guidance.
  - **Caveats:** static popularity metrics; unvetted inclusion quality; fast-moving features.
- [awesome-claude-code-subagents](https://github.com/VoltAgent/awesome-claude-code-subagents) - Curated collection of ready-to-use Claude Code subagents across domains.
  - **Strengths:** wide subagent catalog; multi-domain coverage; drop-in ready definitions.
  - **Caveats:** quality varies per subagent; not uniformly vetted; rapidly evolving.
- [awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) - Curated 1000+ Claude Skills for productivity and coding.
  - **Strengths:** 1000+ production-ready skills; cross-platform compatibility; efficient token-based loading.
  - **Caveats:** activation depends on agent detection; requires API auth; Composio platform dependency.
- [awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) - 100+ AI agent and RAG application templates ready to clone and ship.
  - **Strengths:** hand-built, tested templates; provider-agnostic stack switching; production-ready.
  - **Caveats:** requires third-party API keys; varied frameworks add learning curve.

### Methodologies & Spec-Driven Workflows

- [Agent OS](https://buildermethods.com/agent-os) - Standards-management system that injects coding standards into AI agents.
  - **Strengths:** standards management for AI agents; extracts tribal knowledge; markdown output.
  - **Caveats:** complements (not replaces) tools; full integration only in Claude Code; setup burden.
- [awesome-design-md](https://github.com/VoltAgent/awesome-design-md) - Curated examples of the `DESIGN.md` spec pattern for AI-agent-driven development.
  - **Strengths:** collected `DESIGN.md` exemplars; promotes design-first agent workflows; growing community.
  - **Caveats:** convention not yet standard; usefulness depends on agent's spec-reading capabilities.
- [BMAD-METHOD](https://github.com/bmad-code-org/BMAD-METHOD) - Open-source agentic agile framework with guided workflows from ideation to autonomous implementation.
  - **Strengths:** fully free, open-source; expert-collaborator personas; scale-domain-adaptive planning.
  - **Caveats:** requires CLI invocation (`npx bmad-method@next install`); newer methodology with evolving personas.
- [claude-code-best-practice](https://github.com/shanraisshan/claude-code-best-practice) - Distilled best-practice patterns and conventions for Claude Code teams.
  - **Strengths:** concise reference of community-tested patterns; quick-start for new teams; living doc.
  - **Caveats:** opinionated; may not match every workflow; small maintainer pool.
- [dotnet/skills](https://github.com/dotnet/skills) - Microsoft's curated collection of 11 .NET-specialized agent skills.
  - **Strengths:** domain-specific .NET expertise (EF/MSBuild/NuGet/MAUI/ASP.NET); works with 5+ AI platforms; agentskills.io standard.
  - **Caveats:** .NET-only scope; framework-version coverage and maturity vary by skill.
- [spec-kit](https://github.com/github/spec-kit) - GitHub's open-source spec-driven development toolkit for AI agents.
  - **Strengths:** works with 30+ AI agents; 100+ community extensions; built-in quality gates.
  - **Caveats:** methodology overhead for simple tasks; spec-first discipline required; rapid evolution (281 open issues).

### Skill & Plugin Marketplaces

Web-hosted directories and marketplaces for discovering and installing Skills and Connectors.

- [Claude Connectors](https://claude.com/connectors) - Anthropic's official directory of partner Connectors for Claude.
  - **Strengths:** official Anthropic directory; vetted partners; first-party integrations.
  - **Caveats:** curated to partners only; not for indie skill discovery.
- [SkillHub](https://skillhub.club) - Community hub for discovering and sharing Claude Skills.
  - **Strengths:** discovery-focused; community submissions; lightweight UX.
  - **Caveats:** smaller catalog; uncertain long-term maintenance.
- [Skills.sh](https://skills.sh) - Community library and discovery site for Anthropic Skills.
  - **Strengths:** dedicated Skills directory; web-based discovery; community submissions.
  - **Caveats:** newer platform; coverage and curation still evolving.
- [SkillsMP](https://skillsmp.com) - Community marketplace for sharing and discovering Skills.
  - **Strengths:** searchable index; community-driven submissions; growing catalog.
  - **Caveats:** smaller than Smithery; quality varies per submission.
- [Smithery](https://smithery.ai) - MCP server and Skills marketplace with a one-click install wizard.
  - **Strengths:** large MCP catalog; Skills section; one-click install; popular with agent builders.
  - **Caveats:** MCP-leaning; quality varies; some features paid.

## Agent SDKs & Frameworks

Libraries for building your own agents.

### Official Vendor SDKs

- [Claude Agent SDK (Python)](https://github.com/anthropics/claude-agent-sdk-python) - Anthropic's Python SDK for building agents on the Claude Code agent loop.
  - **Strengths:** mirrors Claude Code's agent loop; built-in tools; MCP server support; eager session-store flushing.
  - **Caveats:** Anthropic-only; pre-1.x breaking changes; Python 3.10+ required.
- [Claude Agent SDK (TypeScript)](https://github.com/anthropics/claude-agent-sdk-typescript) - Anthropic's TypeScript SDK for building agents on the Claude Code agent loop.
  - **Strengths:** typed mirror of the Python SDK; first-class web/Node support; Anthropic-maintained.
  - **Caveats:** Anthropic-only; younger than the Python SDK; some APIs still experimental.
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - Lightweight multi-agent framework with sandbox execution and observability.
  - **Strengths:** small surface area; OpenAI-native tools; voice support; tracing built-in.
  - **Caveats:** OpenAI-leaning; multi-provider support uneven.
- [Vercel AI SDK](https://github.com/vercel/ai) - TypeScript toolkit for agents across React, Next.js, Vue, Node.js, and Svelte.
  - **Strengths:** unified provider API; React/Next-friendly streaming; large template library.
  - **Caveats:** TS/JS only; opinionated about UI patterns.

### Orchestration Frameworks

- [AutoGen / Microsoft Agent Framework](https://github.com/microsoft/autogen) - Microsoft's open-source framework combining multi-agent patterns with enterprise features.
  - **Strengths:** mature multi-agent patterns; group-chat orchestration; Azure-friendly.
  - **Caveats:** consolidation with Microsoft Agent Framework in progress; APIs in flux.
- [CrewAI](https://github.com/crewAIInc/crewAI) - Role-based multi-agent framework with crew coordination and shared context.
  - **Strengths:** intuitive role/crew metaphor; large community; rapid prototyping.
  - **Caveats:** opinionated; best for orchestration patterns it models well.
- [Dify](https://github.com/langgenius/dify) - Open-source LLMOps platform with workflows, RAG, agents, and observability.
  - **Strengths:** comprehensive (workflows/RAG/agents/observability); 50+ pre-built tools; extensive model support.
  - **Caveats:** 2+ cores, 4+ GB RAM minimum; deployment complexity; enterprise features separately licensed.
- [LangChain](https://github.com/langchain-ai/langchain) - High-level framework for building LLM applications with provider-agnostic tool calling.
  - **Strengths:** broad provider support; massive ecosystem; many community integrations.
  - **Caveats:** abstractions can leak; surface area large; performance trade-offs vs LangGraph.
- [LangGraph](https://github.com/langchain-ai/langgraph) - Low-level graph-based orchestration for production stateful agents with checkpointing.
  - **Strengths:** explicit graphs; checkpointing; human-in-the-loop patterns; production-grade.
  - **Caveats:** steeper learning curve than LangChain; verbose for simple agents.
- [LlamaIndex](https://github.com/run-llama/llama_index) - RAG framework with agent workflows and context-aware AI agents.
  - **Strengths:** 300+ integrations; flexible starter or custom packages; 5-line API entry.
  - **Caveats:** README not frequently updated; learning curve with extensive customization; in-memory storage default.
- [Mastra](https://github.com/mastra-ai/mastra) - TypeScript-first agent framework with workflows, memory, and evals.
  - **Strengths:** 40+ provider routing; graph-based workflows; human-in-the-loop; production observability.
  - **Caveats:** TypeScript-only; enterprise features need commercial license; substantial learning curve.
- [Paperclip](https://github.com/paperclipai/paperclip) - Open-source multi-agent orchestration framework aimed at autonomous "zero-human company" operation.
  - **Strengths:** agent-agnostic orchestration primitives; org-chart and routing abstractions over raw prompts; rapid community growth.
  - **Caveats:** aspirational framing (autonomous-company scope); operational/infrastructure setup required; early-stage feature surface.
- [Semantic Kernel](https://github.com/microsoft/semantic-kernel) - Microsoft's open SDK for LLM integration with plugins, prompt templates, and memory.
  - **Strengths:** enterprise-ready; multi-language (Python/C#/Java/TS); Copilot integration.
  - **Caveats:** less agent-native than LangGraph; plugin model less intuitive than LangChain.

### Lightweight & Typed

- [Agno](https://github.com/agno-agi/agno) - Lightweight stateful-agent framework with memory and knowledge (formerly Phidata).
  - **Strengths:** 3-layer production architecture; 100+ integrations; 30-line coding agent; native safety controls.
  - **Caveats:** AgentOS control plane proprietary; telemetry by default; recommended models are high-end.
- [DSPy](https://github.com/stanfordnlp/dspy) - Declarative framework for optimizing reasoning pipelines and agents via program synthesis.
  - **Strengths:** prompt-as-code optimization; provable improvements via compilation; research-backed.
  - **Caveats:** unfamiliar paradigm; debugging optimized programs harder than vanilla prompts.
- [Inngest AgentKit](https://github.com/inngest/agent-kit) - Multi-agent orchestration in TypeScript with MCP tool support and durable workflows.
  - **Strengths:** deterministic routing with control; multi-model providers; MCP integration; local debugging.
  - **Caveats:** TypeScript-only; early-stage ecosystem; explicit orchestration required; learning curve.
- [Mirascope](https://github.com/Mirascope/mirascope) - Provider-agnostic Python toolkit for building autonomous agents with tools and memory.
  - **Strengths:** unified multi-LLM interface; decorated function simplicity; structured Pydantic output.
  - **Caveats:** README documentation depth limited; monorepo complexity; few error-handling examples.
- [Pydantic AI](https://github.com/pydantic/pydantic-ai) - Type-safe Python agent framework with automatic output validation.
  - **Strengths:** Pydantic-native typing; strict structured output; great DX for typed Python codebases.
  - **Caveats:** Python-only; smaller ecosystem than LangChain.
- [Smolagents](https://github.com/huggingface/smolagents) - Hugging Face's minimal agent library with code-writing agents and sandboxing.
  - **Strengths:** very small (<1k lines); code-as-action paradigm; sandbox built in.
  - **Caveats:** newer; thinner integration catalog; less battle-tested.

### Structured Output & Multi-Provider

- [Guidance](https://github.com/guidance-ai/guidance) - Declarative control for LLM generation via guidance language with FSM/regex/grammar constraints.
  - **Strengths:** state-of-the-art structured output; Microsoft Research backing; token efficiency.
  - **Caveats:** steep learning curve for custom grammars; latency for complex constraints.
- [Instructor](https://github.com/567-labs/instructor) - Multi-language structured outputs for LLMs with Pydantic-style validation and retries.
  - **Strengths:** 3M+ monthly downloads; Pydantic-native validation; 15+ provider support; automatic retries.
  - **Caveats:** schema-definition overhead; retry-loop latency; non-Python implementations mature unevenly.
- [LiteLLM](https://github.com/BerriAI/litellm) - Unified LLM API wrapper exposing 100+ models in OpenAI-compatible format with proxy server.
  - **Strengths:** drop-in OpenAI replacement; cost tracking; fallback routing; 100+ providers.
  - **Caveats:** handles model calls only (not full structured output); proxy adds operational layer.
- [Outlines](https://github.com/dottxt-ai/outlines) - Fast structured generation via FSM/regex/grammar; works with Ollama, vLLM, OpenAI.
  - **Strengths:** zero-dependency core; multi-provider; JSON 100% valid guarantee; performance-focused.
  - **Caveats:** newer project; grammar debugging harder than JSON schemas; needs token-level model control.

### Stateful Agents

- [Letta](https://github.com/letta-ai/letta) - Platform for stateful agents with advanced memory management (formerly MemGPT).
  - **Strengths:** advanced self-improving memory; CLI/API/SDK access; model-agnostic; pre-built tooling.
  - **Caveats:** recommended baselines are Opus/GPT-5.2 class; cloud API key mandatory; Node.js 18+ prerequisite.

## Supporting Infrastructure

What agents need to be useful in production.

### Memory

- [agentmemory](https://github.com/rohitg00/agentmemory) - Persistent memory layer that captures, compresses, and replays coding-agent sessions across 15+ tools via MCP.
  - **Strengths:** benchmarked retrieval on LongMemEval-S; broad agent coverage (Claude Code, Cursor, Cline, etc.); zero external databases.
  - **Caveats:** young project with rapidly evolving API; pinned to older iii-engine version.
- [Cognee](https://github.com/topoteretes/cognee) - Memory engine with knowledge graphs, ECL pipeline, and multi-hop reasoning.
  - **Strengths:** unified multi-source ingestion; agent learning across sessions; 4-method simplicity.
  - **Caveats:** hidden complexity behind simplicity; external LLM API dependency; operational maturity questions.
- [context-mode](https://github.com/mksglu/context-mode) - MCP plugin that sandboxes tool output and reduces context window usage via FTS5 indexing.
  - **Strengths:** massive context savings (315KB→5KB examples); hooks across 15+ platforms; growing developer adoption.
  - **Caveats:** sandboxing prevents agent re-reading output; MCP-only; requires hook support or instruction fallback.
- [Mem0](https://github.com/mem0ai/mem0) - Universal memory layer with semantic, BM25, and entity-linked retrieval.
  - **Strengths:** multi-level memory architecture; intuitive cross-platform SDKs; 91%+ benchmark improvements.
  - **Caveats:** LLM provider dependency; embedding-model requirements; self-hosted operational overhead.
- [Zep](https://github.com/getzep/zep) - Long-term memory management for agents with semantic search and summarization.
  - **Strengths:** sub-200ms context assembly; temporal knowledge graphs; multi-language SDKs; SOC2/HIPAA.
  - **Caveats:** WIP status; Community Edition deprecated; cloud-vendor dependency; documentation gaps.

### Vector Databases

- [Chroma](https://github.com/chroma-core/chroma) - Open-source AI embedding database for RAG with native embedding and retrieval.
  - **Strengths:** zero-config local dev; in-memory or disk; multi-language SDKs; large community.
  - **Caveats:** SQLite default limits scale; production hardening ongoing.
- [LanceDB](https://github.com/lancedb/lancedb) - Developer-friendly embedded retrieval library for multimodal AI (Python/JS/Rust).
  - **Strengths:** multimodal (text + images); Apache Arrow backend; fast embedded use; minimal dependencies.
  - **Caveats:** newer than Chroma; smaller adoption; Arrow learning curve for advanced queries.
- [Milvus](https://github.com/milvus-io/milvus) - Cloud-native distributed vector database supporting billions of vectors with GPU acceleration.
  - **Strengths:** massive scale; GPU support; Kubernetes-native; managed cloud via Zilliz.
  - **Caveats:** deployment complexity; operational overhead; overkill for <100M vectors.
- [pgvector](https://github.com/pgvector/pgvector) - PostgreSQL extension for vector similarity search with IVFFlat and HNSW indices.
  - **Strengths:** Postgres-native; no new infra; SQL-native; integrates with existing DBs.
  - **Caveats:** limited to Postgres; slower than specialized DBs at scale; index tuning required.
- [Qdrant](https://github.com/qdrant/qdrant) - High-performance Rust vector database with filtering, reranking, and hybrid search.
  - **Strengths:** sub-100ms latency at scale; production-ready; built-in BM25; gRPC/REST APIs.
  - **Caveats:** memory overhead for large embeddings; Rust backend not customizable; enterprise paywall.
- [Weaviate](https://github.com/weaviate/weaviate) - Vector database with hybrid semantic + keyword search and ML-ready architecture.
  - **Strengths:** GraphQL + REST APIs; combined semantic + keyword search; modular ML plugins.
  - **Caveats:** heavier resource footprint; cloud-first deployment; API complexity.

### Codebase Context

- [ast-grep](https://github.com/ast-grep/ast-grep) - Code search and structural pattern matching tool for codebases.
  - **Strengths:** intuitive AST patterns; Rust performance with multicore; versatile use cases.
  - **Caveats:** language-coverage scope; learning curve for advanced patterns; ecosystem still maturing.
- [Code2Prompt](https://github.com/mufeedvh/code2prompt) - Fast CLI that converts a codebase into LLM-friendly prompts with token counts.
  - **Strengths:** Rust-built performance; token tracking and templating; interactive TUI; Git-aware.
  - **Caveats:** docs reliance; purpose-built for LLM context only; feature set still stabilizing.
- [context-hub](https://github.com/andrewyng/context-hub) - Context-management tool that organizes codebase information into structured docs with agent feedback loops.
  - **Strengths:** local note persistence across sessions; feedback-driven doc improvement; markdown-based; CLI via npm.
  - **Caveats:** requires manual curation of doc structure; external API dependencies for some features.
- [Context7](https://github.com/upstash/context7) - Up-to-date version-specific documentation injection for LLMs via CLI or MCP.
  - **Strengths:** version-specific docs prevent hallucinated APIs; works with 30+ AI clients.
  - **Caveats:** community-contributed library quality not guaranteed; private supporting components; API-key dependency.
- [GitIngest](https://github.com/coderamp-labs/gitingest) - Lightweight tool that prepares Git repositories for LLM context windows.
  - **Strengths:** simple URL transformation for repos; web/extension/CLI/package access; respects `.gitignore`.
  - **Caveats:** GitHub-token setup friction; no explicit large-codebase optimization; Python 3.8+ required.
- [GitNexus](https://github.com/abhigyanpatwari/GitNexus) - Client-side knowledge-graph engine for repos with zero-server, in-browser indexing.
  - **Strengths:** precomputed knowledge graphs enable smaller models; 14+ languages; local-first privacy.
  - **Caveats:** web UI capped at 5000 files; incomplete language features; commercial lock-in for advanced features.
- [MarkItDown](https://github.com/microsoft/markitdown) - CLI and Python library that converts PDFs, Office docs, images, and audio into LLM-ready Markdown.
  - **Strengths:** broad format coverage (PDF, Office, images, audio); Microsoft-maintained; widely adopted ingest tool.
  - **Caveats:** general-purpose ingestion (not code-specific); audio transcription needs external API like Whisper.
- [Repomix](https://github.com/yamadashy/repomix) - AI-friendly codebase packing with tree-sitter compression for big token reductions.
  - **Strengths:** AI-optimized formatting; 70% compression via tree-sitter; security scanning; flexible deployment.
  - **Caveats:** compression feature experimental; configuration complexity; remote config untrusted.
- [semgrep](https://github.com/semgrep/semgrep) - Lightweight static analysis for 30+ languages with natural-syntax pattern matching.
  - **Strengths:** agent-friendly patterns; 2000+ community rules; self-hostable; CLI-first.
  - **Caveats:** slower than specialized linters; not for high-volume checks; rule quality varies.
- [tree-sitter](https://github.com/tree-sitter/tree-sitter) - Incremental parsing library for 50+ languages, powering VS Code/GitHub/LSP tooling.
  - **Strengths:** incremental parsing (efficient for long files); language-agnostic; widely adopted.
  - **Caveats:** C library (bindings needed for Python/JS); no semantic analysis; grammar maintenance burden.

### Sandboxing & Execution

- [Daytona](https://github.com/daytonaio/daytona) - Sub-90ms sandbox creation for AI-generated code with lifecycle automation.
  - **Strengths:** sub-90ms startup; multi-language SDKs; full isolation; persistent state snapshots.
  - **Caveats:** AGPL-3.0 restrictions; Python/TypeScript/JS runtimes only; Docker/PostgreSQL deployment complexity.
- [E2B](https://github.com/e2b-dev/E2B) - Open-source cloud sandboxes via Firecracker for secure AI code execution.
  - **Strengths:** JS/TS and Python SDKs; minimal code to spin sandboxes; Code Interpreter capability.
  - **Caveats:** primarily cloud-dependent; documentation gaps; self-hosting requires infra expertise.
- [Modal](https://modal.com) - gVisor-based sandboxes with sub-second starts and deny-by-default networking (proprietary).
  - **Strengths:** sub-second cold starts; ~100x faster than Docker for AI; GPU elasticity; code-first Python.
  - **Caveats:** specialized for AI/ML; Python-centric; free tier capped at $30/month.
- [Riza](https://riza.io) - Secure sandboxing runtime for AI-generated code (proprietary).
  - **Strengths:** <10ms execution startup; billions of monthly executions; isolated execution; REST API.
  - **Caveats:** Python/TypeScript/Go only; self-hosting requires Kubernetes; pricing/limits unclear.
- [Stagehand](https://github.com/browserbase/stagehand) - TypeScript and Python SDK for browser agents using natural-language act/extract/observe primitives.
  - **Strengths:** natural-language browser primitives (act, extract, observe); TypeScript and Python SDKs; widely adopted browser-agent reference.
  - **Caveats:** requires a Chromium-compatible browser environment; advanced features integrate with Browserbase's hosted cloud.
- [Vercel Sandbox](https://vercel.com/docs/vercel-sandbox) - Lightweight sandbox execution integrated with Vercel infrastructure (proprietary).
  - **Strengths:** millisecond startup; Node24 / Python 3.13 runtimes; snapshotting; persistent beta support.
  - **Caveats:** Amazon Linux 2023 only; documentation thin; Firecracker VM constraints.

### Workflow & Pipeline Orchestration

- [Dagger](https://github.com/dagger/dagger) - Containerized pipelines as code (TypeScript/Go/Python) that run locally, in CI, or cloud.
  - **Strengths:** portable execution; reduces CI vendor lock-in; code-first vs YAML; Docker-native.
  - **Caveats:** smaller ecosystem vs Jenkins/GitHub Actions; learning curve; not AI-specific.
- [Flowise](https://github.com/FlowiseAI/Flowise) - Visual low-code LLM app builder with drag-drop workflows for agents, RAG, and chatbots.
  - **Strengths:** AI/LLM-specific; low-code; 200+ integrations; Docker-easy deploy.
  - **Caveats:** not production-scale; limited orchestration patterns; rapid feature churn.
- [Kestra](https://github.com/kestra-io/kestra) - Event-driven workflow orchestration with YAML; real-time scheduling, retries, sub-flows.
  - **Strengths:** event-driven triggers; language-agnostic; 300+ integrations; enterprise-ready.
  - **Caveats:** YAML learning curve; less AI-specific than Flowise; self-hosting complexity.
- [n8n](https://github.com/n8n-io/n8n) - Fair-code workflow automation with 1000+ native integrations and hybrid visual + code editor.
  - **Strengths:** largest integration count; self-hostable; visual + code editor; community + enterprise tiers.
  - **Caveats:** performance not AI-optimized; broad scope adds learning surface; enterprise UX.
- [Prefect](https://github.com/PrefectHQ/prefect) - Pythonic workflow orchestration for data pipelines with growing AI/agent positioning.
  - **Strengths:** Pythonic; serverless-ready; agent monitoring via Marvin; cloud UI.
  - **Caveats:** data-pipeline origin (not agent-native); steeper learning curve than Kestra.

### Evaluation

- [Braintrust](https://www.braintrust.dev) - Eval lifecycle platform with monitoring, collaboration, and release enforcement (proprietary).
  - **Strengths:** real-time prompt/response inspection; side-by-side comparisons; Brainstore proprietary DB; SOC2/HIPAA.
  - **Caveats:** premium pricing likely; vendor integration required; documented limits sparse.
- [DeepEval](https://github.com/confident-ai/deepeval) - Local LLM evaluation framework with agent-specific metrics.
  - **Strengths:** large set of ready metrics; local execution; framework-agnostic; pytest-style.
  - **Caveats:** requires `OPENAI_API_KEY`; accuracy benchmarks undocumented; setup complexity for custom metrics.
- [Inspect AI](https://github.com/UKGovernmentBEIS/inspect_ai) - UK AI Safety Institute's framework with 200+ pre-built evals for agents and reasoning.
  - **Strengths:** 200+ pre-built evals; extensive built-ins; extensible; comprehensive docs.
  - **Caveats:** TypeScript frontend requires separate setup; complex initial config; multiple maintenance dependencies.
- [Promptfoo](https://github.com/promptfoo/promptfoo) - Red-teaming and evaluation for prompts, agents, and RAG.
  - **Strengths:** fast local eval with caching; multi-provider; red-teaming built in; MIT licensed.
  - **Caveats:** Node.js 20.20+ required; most providers need API keys; large-scale limits unclear.
- [RAGAS](https://github.com/vibrantlabsai/ragas) - Automated evaluation for RAG and agent systems with tool-call and goal-accuracy metrics.
  - **Strengths:** objective metrics for RAG/agents; automatic test generation; LangChain integrations.
  - **Caveats:** limited template availability; depends on external LLMs; documentation incomplete.

### Observability

- [Helicone](https://github.com/Helicone/helicone) - Open-source LLM observability platform for tracing and monitoring.
  - **Strengths:** 100+ models via single API key; one-line integration; comprehensive observability; self-hosting option.
  - **Caveats:** documentation timeliness issues; manual deployment not recommended; provider gaps possible.
- [Langfuse](https://github.com/langfuse/langfuse) - Open-source observability with tracing, evals, and prompt management.
  - **Strengths:** integrated LLMOps suite; flexible deployment (cloud/Docker/Kubernetes); battle-tested at scale.
  - **Caveats:** telemetry enabled by default; enterprise features under separate license; external LLM dependency.
- [Lunary](https://lunary.ai) - Prompt versioning, monitoring, and experimentation with agent-behavior visualization.
  - **Strengths:** open-source; agent-behavior trees; prompt versioning and A/B; self-hostable.
  - **Caveats:** smaller ecosystem than Langfuse/Helicone; some features behind paid plans.
- [OpenLLMetry](https://github.com/traceloop/openllmetry) - OpenTelemetry-based agent observability for 20+ providers.
  - **Strengths:** 25+ observability platform destinations; standards-based OpenTelemetry; comprehensive LLM coverage.
  - **Caveats:** Python SDK primary; fragmented JavaScript ecosystem; telemetry-privacy docs needed.
- [Opik](https://github.com/comet-ml/opik) - Open-source LLM observability with tracing, automated evals, and production dashboards from Comet ML.
  - **Strengths:** combines tracing, evals, and dashboards in one stack; Comet-backed and Apache-2.0; strong RAG and agentic-workflow coverage.
  - **Caveats:** smaller ecosystem than Langfuse/Helicone; some advanced features tied to Comet's hosted platform.
- [Phoenix](https://github.com/Arize-ai/phoenix) - Arize's open-source LLM observability platform for tracing and evaluation.
  - **Strengths:** unified tracing/evaluation/datasets/experiments; OpenTelemetry standards; flexible deployment.
  - **Caveats:** Elastic License restrictions; telemetry enabled by default; self-hosting needs containerization.

### Prompt Management

- [Agenta](https://github.com/Agenta-AI/agenta) - LLMOps platform with Git-like prompt versioning and parallel experimentation.
  - **Strengths:** integrated prompt/eval/observability; 50+ LLM models; custom + pre-built evaluators.
  - **Caveats:** learning curve for feature breadth; self-hosting Docker complexity; telemetry default-enabled.
- [Latitude](https://github.com/latitude-dev/latitude-llm) - Enterprise prompt engineering with collaboration and real-time validation.
  - **Strengths:** issue-centric error tracking; human-aligned evaluations; agent-native multi-turn visibility.
  - **Caveats:** alpha stage, not production-ready; incomplete roadmap; Python/Go support underdocumented.
- [PromptLayer](https://promptlayer.com) - Prompt management and analytics with versioning and A/B testing (proprietary).
  - **Strengths:** version/test/monitor in one; visual editor; collaborative design; enterprise focus.
  - **Caveats:** limited public technical documentation; vague implementation details; sparse samples.

### Benchmarks & Leaderboards

- [Aider Polyglot Leaderboard](https://aider.chat/docs/leaderboards/) - Aider's leaderboard ranking models on multi-language code editing tasks.
  - **Strengths:** 225 polyglot exercises; evaluates editing not just generation; transparent cost/token metrics.
  - **Caveats:** narrow task scope; exercise-based testing may not generalize; cost-vs-performance trade-offs.
- [LiveCodeBench](https://livecodebench.github.io) - Holistic benchmark for code LLMs with contamination-free, dynamically updated problems.
  - **Strengths:** contamination-free post-cutoff data; holistic assessment including self-repair.
  - **Caveats:** 300+ problems may be insufficient; competitive-programming bias; limited mechanism analysis.
- [SWE-bench](https://www.swebench.com) - Benchmark of real-world GitHub issues that agents must resolve end-to-end.
  - **Strengths:** multiple benchmark variants; comparative agent analysis; filtering by agent/model type.
  - **Caveats:** methodology details sparse in public docs; results vary widely by harness.
- [SWE-bench Verified](https://openai.com/index/introducing-swe-bench-verified/) - OpenAI-curated subset of SWE-bench with human-validated solutions.
  - **Strengths:** human-validated tasks; cleaner signal than raw SWE-bench; widely cited as the comparison standard.
  - **Caveats:** still subset of GitHub issues; vendor-curated; can be gamed by overfitting.
- [Terminal-Bench](https://www.tbench.ai) - Benchmark for agents performing real tasks inside a terminal.
  - **Strengths:** diverse domains (ML/security/data science); practical real-world tasks; multiple versions.
  - **Caveats:** terminal environments only; incomplete leaderboard transparency; v3.0 still in progress.

### Test Generation

- [Diffblue Cover](https://www.diffblue.com) - Reinforcement-learning unit test generator focused on Java/Kotlin (proprietary).
  - **Strengths:** enterprise unit-test automation; AI testing agent positioning; SOC2/compliance capable.
  - **Caveats:** documentation thin in public; benchmark claims not independently verified; pricing unclear.

### Local LLM Runners

These back local coding agents (e.g., aider with Ollama, Continue with local models). Included because most agent toolchains hit them sooner or later.

- [llama.cpp](https://github.com/ggml-org/llama.cpp) - Lightweight C++ LLM inference with minimal dependencies.
  - **Strengths:** plain C/C++ minimal deps; 1.5–8 bit quantization; Apple Silicon optimized; multicore.
  - **Caveats:** inference-only (no training); GGUF format conversion required; hardware-specific optimization.
- [Llamafile](https://github.com/mozilla-ai/llamafile) - Single-file executable bundling model and runtime via Cosmopolitan.
  - **Strengths:** single-file executable; no install needed; cross-platform; bundled whisperfile.
  - **Caveats:** newer versions may lack prior features; version fragmentation; GPU recommended.
- [Ollama](https://github.com/ollama/ollama) - Single-binary LLM server with built-in model registry and GPU detection.
  - **Strengths:** easy install/use; 100+ model support; 100+ integrations; API-first with libraries.
  - **Caveats:** hardware/resource requirements undocumented; performance benchmarks absent; no production guarantees.
- [vLLM](https://github.com/vllm-project/vllm) - High-throughput Python LLM server with PagedAttention.
  - **Strengths:** state-of-the-art throughput; PagedAttention; 200+ model architectures; GPU/CPU/TPU.
  - **Caveats:** hardware dependency for optimal perf; configuration complexity for advanced features.

## Learning Resources

### Articles & Blogs

- [Anthropic Engineering Blog](https://www.anthropic.com/engineering) - Anthropic's posts on agents, Claude Code, and the Agent SDK.
  - **Strengths:** primary source on Claude Code internals and agent patterns; deep technical posts.
  - **Caveats:** Anthropic-focused; pacing varies.
- [Simon Willison's Blog](https://simonwillison.net) - Hands-on coverage of LLMs, agents, Claude Skills, and prompt engineering.
  - **Strengths:** rigorous, hands-on coverage; tracks the entire LLM/agent ecosystem; archive deep.
  - **Caveats:** opinionated single-author voice; daily firehose volume.

### Tutorials & Courses

- [AI Agents for Beginners](https://github.com/microsoft/ai-agents-for-beginners) - Microsoft's free 11-lesson course on building AI agents with frameworks and patterns.
  - **Strengths:** free; 11 structured lessons; multi-language translations; production-quality docs.
  - **Caveats:** Microsoft/Azure-leaning examples; beginner pacing.
- [GenAI Agents](https://github.com/NirDiamant/GenAI_Agents) - Tutorials and reference implementations covering AI agent techniques and architectures.
  - **Strengths:** 50+ agent implementations; covers planning/tool-use/multi-agent patterns; active community.
  - **Caveats:** Python-centric; tutorial depth varies.
- [Prompt Engineering Guide](https://github.com/dair-ai/Prompt-Engineering-Guide) - Curated reference for prompt engineering techniques, papers, and tools.
  - **Strengths:** canonical reference; covers techniques + papers; multi-language translations.
  - **Caveats:** broad over deep; frontier-model improvements outdate sections quickly.
- [RAG Techniques](https://github.com/NirDiamant/RAG_Techniques) - Comprehensive collection of RAG implementation patterns from basic to advanced.
  - **Strengths:** wide pattern coverage; hands-on notebooks; widely referenced in the community.
  - **Caveats:** Python/LangChain bias; deep on RAG but narrow on broader agent work.

### Books

- [AI Engineering](https://www.oreilly.com/library/view/ai-engineering/9781098166298/) - Chip Huyen's reference covering agents, evals, tools, and production patterns.
  - **Strengths:** broad practitioner reference; agents/evals chapters strong; covers production patterns.
  - **Caveats:** rapid field evolution dates parts; less depth on coding-agent specifics than dedicated tools.

### Podcasts

- [Latent Space](https://www.latent.space/podcast) - Deep-dive interviews with builders of coding agents, MCP, SWE-bench, and frontier teams.
  - **Strengths:** interviews with primary sources; coding-agent and infra emphasis; transcripts available.
  - **Caveats:** Bay Area / vendor-heavy guest mix; long episodes.

### Datasets

- [Cleaned Alpaca Dataset](https://github.com/gururise/AlpacaDataCleaned) - Cleaned Alpaca instruction dataset for fine-tuning LLMs.
  - **Strengths:** 9.5% perplexity improvement; 40% higher truthfulness; 52k entries; open contribution.
  - **Caveats:** quality issues remain; ~80% math problems still incorrect; some long tokens.

## Community

- [Anthropic on X](https://x.com/AnthropicAI) - Updates from Anthropic on Claude and Claude Code.
- [Cursor Forum](https://forum.cursor.com) - Official community forum for Cursor users.
- [r/ChatGPTCoding](https://www.reddit.com/r/ChatGPTCoding/) - Subreddit covering AI coding tools across vendors.

## About

Inspired by [awesome](https://github.com/sindresorhus/awesome), [awesome-dotnet-core](https://github.com/thangchung/awesome-dotnet-core), [awesome-ai-agents](https://github.com/jim-schwoebel/awesome_ai_agents), and [awesome-claude-code](https://github.com/hesreallyhim/awesome-claude-code).

Contributions are always welcome! Use the issue templates to suggest a new tool or flag an outdated one — we accept proprietary and commercial software too, as long as it has visible community use.

Thanks to all contributors — you're awesome and this wouldn't be possible without you. The goal is to build a categorized, community-driven collection of well-known tools, libraries, MCP servers, and frameworks that power AI coding agents.

---

<div align="center">

### 💖 Show Your Support

If this list helped you, give it a ⭐ and share it with your team.
Contributions welcome via [Issues](../../issues) and [Pull Requests](../../pulls).

<sub>Made with ❤ for the AI coding community</sub>

</div>
