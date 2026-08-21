# Awesome AI Agents

> A curated collection of AI agents, agent platforms, frameworks, and infrastructure.

<!-- counts:start -->
![Entries](https://img.shields.io/badge/entries-96-informational)
![Categories](https://img.shields.io/badge/categories-12-informational)
<!-- counts:end -->
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen)
[![License: CC BY 4.0](https://img.shields.io/badge/license-CC%20BY%204.0-lightgrey)](LICENSE)

Most agent lists put a chatbot, a Python library, and a sandbox provider in the same section
and leave the reader to work out which is which. This one does not. The categories separate
agents you point at a task, frameworks you build with, and infrastructure you run underneath,
because those are three different shopping trips.

The bar for inclusion is that something takes several steps on its own and acts outside the
chat window. Assistants that answer well but do nothing are not here, however capable they
are. Projects that were prominent in the first agent wave and have since stopped moving are
not here either.

Maintained by [TiorAI](https://tiorai.com/), which catalogues AI tools for a living.

<!-- last-reviewed:start -->
**Last reviewed:** 2026-08-21
<!-- last-reviewed:end -->

## Contents

- [Coding agents](#coding-agents)
- [Browser and computer-use agents](#browser-and-computer-use-agents)
- [Research agents](#research-agents)
- [Customer support agents](#customer-support-agents)
- [Sales and outbound agents](#sales-and-outbound-agents)
- [Data and analytics agents](#data-and-analytics-agents)
- [Workflow automation agents](#workflow-automation-agents)
- [Agent building platforms](#agent-building-platforms)
- [Agent frameworks](#agent-frameworks)
- [Multi-agent orchestration](#multi-agent-orchestration)
- [Agent infrastructure](#agent-infrastructure)
- [Evaluation and observability](#evaluation-and-observability)
- [How agents are selected](#how-agents-are-selected)
- [Suggest an agent](#suggest-an-agent)
- [Contributing](#contributing)
- [Disclaimer](#disclaimer)
- [License](#license)
- [About TiorAI](#about-tiorai)

## Coding agents

Agents that read a repository, write changes, and run what they wrote.

- **[Aider](https://aider.chat/)** — Terminal agent that edits files in a local git repository and makes a commit for each change. `Open Source` `CLI`
- **[Claude Code](https://www.claude.com/product/claude-code)** — Anthropic's terminal agent, which explores a codebase, edits files, and runs tests before reporting back. `Paid` `CLI` `VS Code` `JetBrains`
- **[Cline](https://cline.bot/)** — VS Code agent that plans a change, runs commands, and asks for approval at each step. `Open Source` `VS Code`
- **[Codex CLI](https://developers.openai.com/codex/cli/)** — OpenAI's terminal coding agent, running locally against your repository with a sandboxed execution mode. `Open Source` `CLI`
- **[Devin](https://devin.ai/)** — Cognition's hosted coding agent, given a task and a repository and left to open a pull request. `Paid` `Web` `Windows` `macOS` `Linux`
- **[Goose](https://block.github.io/goose/)** — Block's local agent, which runs on your machine and connects to tools through Model Context Protocol servers. `Open Source` `Windows` `macOS` `Linux` `CLI`
- **[Jules](https://jules.google/)** — Google's asynchronous coding agent, which clones a repository into a cloud VM and proposes a diff. `Freemium` `Web`
- **[OpenHands](https://www.all-hands.dev/)** — Software agent that opens files, runs tests, and iterates inside a sandbox you host yourself. `Open Source` `Web` `CLI`
- **[Roo Code](https://roocode.com/)** — VS Code agent with separate modes for architecture, implementation, and debugging, using your own model key. `Open Source` `VS Code`
- **[SWE-agent](https://swe-agent.com/)** — Princeton research agent that fixes GitHub issues, and the reference implementation most benchmarks compare against. `Open Source` `CLI`

## Browser and computer-use agents

Agents that drive a real browser or desktop rather than calling an API.

- **[Browserbase](https://www.browserbase.com/)** — Hosted headless browsers for agents, with session recording, stealth options, and proxy handling. `Freemium` `Web` `API`
- **[Browser Use](https://browser-use.com/)** — Library that lets an agent drive a real browser, with the page structure exposed as text. `Open Source` `API` `CLI`
- **[Hyperbrowser](https://www.hyperbrowser.ai/)** — Browser infrastructure for agents, with scraping, crawling, and session management behind one API. `Freemium` `Web` `API`
- **[Notte](https://notte.cc/)** — Turns a web page into a structured action space an agent can navigate without brittle selectors. `Open Source` `API` `CLI`
- **[Playwright MCP](https://github.com/microsoft/playwright-mcp)** — Microsoft's Model Context Protocol server exposing Playwright browser control to any compatible agent. `Open Source` `API` `CLI`
- **[Skyvern](https://www.skyvern.com/)** — Automates browser workflows using vision, so a changed layout does not break the run. `Open Source` `Web` `API`
- **[Stagehand](https://www.stagehand.dev/)** — Browser automation framework mixing written Playwright code with natural-language steps where the page varies. `Open Source` `API` `CLI`
- **[Steel](https://steel.dev/)** — Open-source browser API built for agent sessions, self-hostable or run as a managed service. `Open Source` `Web` `API`

## Research agents

Agents that search, read, and synthesise sources into something citable.

- **[Consensus](https://consensus.app/)** — Searches peer-reviewed literature and reports what the weight of evidence says on a question. `Freemium` `Web`
- **[Elicit](https://elicit.com/)** — Runs a literature review as a pipeline, extracting findings from each paper into a comparable table. `Freemium` `Web`
- **[GPT Researcher](https://gptr.dev/)** — Open-source agent that plans queries, reads sources, and writes a cited report on a topic. `Open Source` `Web` `API` `CLI`
- **[Perplexity](https://www.perplexity.ai/)** — Answer engine whose research mode runs many searches and returns a sourced report rather than a snippet. `Freemium` `Web` `iOS` `Android`
- **[STORM](https://storm.genie.stanford.edu/)** — Stanford system that researches a topic from multiple perspectives and drafts a Wikipedia-style article. `Open Source` `Web`
- **[Undermind](https://www.undermind.ai/)** — Scientific literature search that runs a long, iterative crawl instead of returning results immediately. `Freemium` `Web`
- **[You.com](https://you.com/)** — Search product with a research mode that decomposes a question and cites what it used. `Freemium` `Web` `API`

## Customer support agents

Agents that resolve support tickets rather than deflecting them.

- **[Ada](https://www.ada.cx/)** — Support automation platform that resolves conversations across chat, email, and voice channels. `Paid` `Web` `API`
- **[Decagon](https://decagon.ai/)** — Support agent that handles tickets end to end and hands over with full context when it cannot. `Paid` `Web` `API`
- **[Fin](https://fin.ai/)** — Intercom's support agent, which answers from your help content and reports a measured resolution rate. `Paid` `Web` `API`
- **[Forethought](https://forethought.ai/)** — Triages, routes, and resolves support tickets inside an existing helpdesk rather than replacing it. `Paid` `Web` `API`
- **[Gorgias](https://www.gorgias.com/)** — Support platform for online stores, with an agent that handles order and returns questions. `Paid` `Web` `API`
- **[Parloa](https://www.parloa.com/)** — Voice and chat agents for contact centres, aimed at call handling rather than text-only support. `Paid` `Web` `API`
- **[Sierra](https://sierra.ai/)** — Customer-facing agents built per company, with guardrails and outcome-based pricing. `Paid` `Web` `API`
- **[Zendesk AI agents](https://www.zendesk.com/service/ai/)** — Zendesk's own resolution agents, useful mainly if the helpdesk is already there. `Paid` `Web` `API`

## Sales and outbound agents

Agents that research accounts, write outreach, and work a pipeline.

- **[11x](https://www.11x.ai/)** — Outbound sales agent that researches prospects, drafts sequences, and books meetings. `Paid` `Web`
- **[AiSDR](https://aisdr.com/)** — Outbound agent that personalises email from public signals and handles the reply thread. `Paid` `Web`
- **[Artisan](https://www.artisan.co/)** — Sales agent plus the data and sending infrastructure to run outbound without a separate stack. `Paid` `Web`
- **[Clay](https://www.clay.com/)** — Enriches account lists from many data sources and runs research agents over each row. `Freemium` `Web` `API`
- **[Qualified](https://www.qualified.com/)** — Website agent that engages visitors, qualifies them, and books meetings straight into a calendar. `Paid` `Web`
- **[Regie.ai](https://www.regie.ai/)** — Prospecting agent that generates sequences and works the low-priority half of a lead list. `Paid` `Web`
- **[Unify](https://www.unifygtm.com/)** — Finds accounts showing buying intent and runs research and outreach agents against them. `Paid` `Web`

## Data and analytics agents

Agents that query data, write the SQL, and explain the result.

- **[Databricks Genie](https://www.databricks.com/product/ai-bi)** — Conversational analytics over a lakehouse, generating queries and showing the ones it ran. `Paid` `Web`
- **[Hex](https://hex.tech/)** — Notebook platform whose agent writes and edits analysis cells you can inspect and rerun. `Freemium` `Web`
- **[Julius](https://julius.ai/)** — Analyses uploaded spreadsheets in conversation and shows the Python it executed for each answer. `Freemium` `Web`
- **[Vanna](https://vanna.ai/)** — Trains a text-to-SQL agent on your own schema and query history, self-hosted. `Open Source` `API` `CLI`
- **[Wren AI](https://getwren.ai/)** — Open-source analytics agent with a semantic layer, so answers follow your own metric definitions. `Open Source` `Web` `API`

## Workflow automation agents

Agents built into workflow tools, where a step can decide instead of following a rule.

- **[Activepieces](https://www.activepieces.com/)** — Open-source automation platform with agent steps and a large library of connectors. `Open Source` `Web` `API`
- **[Dify](https://dify.ai/)** — Builds and hosts agent workflows with a visual editor, retrieval, and observability included. `Open Source` `Web` `API`
- **[Gumloop](https://www.gumloop.com/)** — Node-based automation aimed at non-developers, with agent nodes for the steps that need judgement. `Freemium` `Web`
- **[Lindy](https://www.lindy.ai/)** — Builds assistants that watch a trigger, then handle email, meetings, and follow-up without supervision. `Freemium` `Web`
- **[Make](https://www.make.com/)** — Visual automation platform with agent modules that choose which scenario branch to run. `Freemium` `Web` `API` · [vs n8n](https://tiorai.com/compare/make-vs-n8n/)
- **[n8n](https://n8n.io/)** — Source-available workflow automation you can self-host, with first-class agent and tool nodes. `Freemium` `Web` `API`
- **[Relay.app](https://www.relay.app/)** — Automation with human approval steps built in, which matters when an agent acts on customer data. `Freemium` `Web`
- **[Zapier Agents](https://zapier.com/agents)** — Agents with access to Zapier's connector library, so they can act across thousands of applications. `Freemium` `Web` · [vs n8n](https://tiorai.com/compare/zapier-ai-vs-n8n/)

## Agent building platforms

Hosted builders for people who would rather not start from a library.

- **[Amazon Bedrock Agents](https://aws.amazon.com/bedrock/agents/)** — Managed agents on AWS, with action groups, knowledge bases, and IAM-scoped permissions. `Paid` `Web` `API`
- **[Botpress](https://botpress.com/)** — Conversational agent builder with a visual flow editor and deployment across common channels. `Freemium` `Web` `API`
- **[Copilot Studio](https://www.microsoft.com/en-us/microsoft-copilot/microsoft-copilot-studio)** — Microsoft's agent builder, aimed at organisations already inside Microsoft 365 and Power Platform. `Paid` `Web`
- **[Dust](https://dust.tt/)** — Team platform for building agents over internal documents and tools, with per-agent permissions. `Paid` `Web` `API`
- **[Flowise](https://flowiseai.com/)** — Drag-and-drop builder for agent and retrieval pipelines, self-hostable and source-available. `Freemium` `Web` `API`
- **[Langflow](https://www.langflow.org/)** — Visual editor for agent flows that exports to Python, so the prototype is not a dead end. `Open Source` `Web` `API`
- **[Vellum](https://www.vellum.ai/)** — Builds and versions agent workflows with evaluation attached, aimed at teams shipping to production. `Paid` `Web` `API`
- **[Vertex AI Agent Builder](https://cloud.google.com/products/agent-builder)** — Google Cloud's managed agent stack, with grounding in Search and enterprise data connectors. `Paid` `Web` `API`

## Agent frameworks

Libraries for building a single agent in code.

- **[Agno](https://www.agno.com/)** — Python framework focused on fast agent instantiation, with memory, tools, and knowledge built in. `Open Source` `API` `CLI`
- **[Google ADK](https://google.github.io/adk-docs/)** — Google's agent development kit, model-agnostic despite the name, with an evaluation harness included. `Open Source` `API` `CLI`
- **[Haystack](https://haystack.deepset.ai/)** — Pipeline framework for retrieval and agents, with components you can swap without rewriting the graph. `Open Source` `API`
- **[LangChain](https://www.langchain.com/)** — The most widely used agent library, and the one with the largest set of existing integrations. `Open Source` `API`
- **[LlamaIndex](https://www.llamaindex.ai/)** — Framework centred on connecting agents to your own documents and structured data. `Open Source` `API`
- **[Mastra](https://mastra.ai/)** — TypeScript agent framework with workflows, memory, and evaluation, aimed at web application developers. `Open Source` `API`
- **[OpenAI Agents SDK](https://openai.github.io/openai-agents-python/)** — OpenAI's minimal agent library, built around handoffs, guardrails, and tracing rather than a large abstraction. `Open Source` `API`
- **[Pydantic AI](https://ai.pydantic.dev/)** — Agent framework that types every input and output, so failures surface at the boundary. `Open Source` `API`
- **[Semantic Kernel](https://learn.microsoft.com/en-us/semantic-kernel/)** — Microsoft's agent SDK for .NET, Python, and Java, aimed at existing enterprise codebases. `Open Source` `API`
- **[smolagents](https://huggingface.co/docs/smolagents/)** — Hugging Face's small agent library, where the agent writes Python instead of emitting tool JSON. `Open Source` `API`
- **[Strands Agents](https://strandsagents.com/)** — AWS-backed framework that leans on the model to plan, keeping the surrounding code small. `Open Source` `API`

## Multi-agent orchestration

Frameworks whose main abstraction is several agents working together.

- **[AutoGen](https://microsoft.github.io/autogen/)** — Microsoft Research framework for conversations between agents, with an event-driven core. `Open Source` `API`
- **[CAMEL](https://www.camel-ai.org/)** — Research framework for studying how large populations of agents behave when they cooperate. `Open Source` `API`
- **[CrewAI](https://www.crewai.com/)** — Assigns roles and tasks to a crew of agents, with sequential or hierarchical execution. `Open Source` `API`
- **[LangGraph](https://www.langchain.com/langgraph)** — Models an agent system as a graph with explicit state, which makes loops and retries debuggable. `Open Source` `API`
- **[MetaGPT](https://www.deepwisdom.ai/)** — Assigns software-company roles to agents and passes structured documents between them. `Open Source` `API`
- **[OpenAI Swarm](https://github.com/openai/swarm)** — The educational predecessor to the Agents SDK, kept for its handoff pattern rather than production use. `Open Source` `API`
- **[OpenServ](https://openserv.ai/)** — Platform for composing specialised agents into a team with shared task state. `Freemium` `Web` `API`

## Agent infrastructure

Sandboxes, tool connectors, memory, and the plumbing agents run on.

- **[Arcade](https://www.arcade.dev/)** — Tool platform that handles user authorisation, so an agent acts as the user rather than a shared key. `Freemium` `API`
- **[Composio](https://composio.dev/)** — Managed connectors to hundreds of applications with authentication handled, exposed as agent tools. `Freemium` `API`
- **[Daytona](https://www.daytona.io/)** — Fast-starting sandboxes for agent-generated code, with a stateful filesystem between runs. `Freemium` `API` `CLI`
- **[E2B](https://e2b.dev/)** — Secure cloud sandboxes where agents can run generated code without touching your infrastructure. `Freemium` `API` `CLI`
- **[Letta](https://www.letta.com/)** — Agent server built around persistent memory, so state survives beyond a single conversation. `Open Source` `Web` `API`
- **[Mem0](https://mem0.ai/)** — Memory layer that decides what to keep from a conversation and recalls it in later sessions. `Open Source` `API`
- **[Modal](https://modal.com/)** — Serverless compute for Python, widely used to run agent workloads and inference on demand. `Freemium` `API` `CLI`
- **[Model Context Protocol](https://modelcontextprotocol.io/)** — Open standard for connecting agents to tools and data, now supported across most major clients. `Open Source` `API` `CLI`
- **[Temporal](https://temporal.io/)** — Durable execution engine that survives crashes and restarts, useful for agents running for hours. `Open Source` `API` `CLI`
- **[Zep](https://www.getzep.com/)** — Memory service that builds a temporal knowledge graph from conversations rather than storing raw text. `Freemium` `API`

## Evaluation and observability

Seeing what an agent did, and telling whether it did it well.

- **[AgentOps](https://www.agentops.ai/)** — Session replay and cost tracking built specifically around agent runs rather than single calls. `Freemium` `Web` `API`
- **[Braintrust](https://www.braintrust.dev/)** — Evaluation platform pairing datasets with scorers, so a prompt change can be measured before shipping. `Freemium` `Web` `API`
- **[Helicone](https://www.helicone.ai/)** — Proxy-based logging for model calls, with caching and cost attribution, self-hostable. `Open Source` `Web` `API`
- **[Langfuse](https://langfuse.com/)** — Open-source tracing, evaluation, and prompt management, run as a service or on your own cluster. `Open Source` `Web` `API`
- **[LangSmith](https://www.langchain.com/langsmith)** — Tracing and evaluation from the LangChain team, and framework-agnostic despite the origin. `Freemium` `Web` `API`
- **[Phoenix](https://phoenix.arize.com/)** — Open-source tracing and evaluation built on OpenTelemetry, so it fits existing observability stacks. `Open Source` `Web` `API`
- **[Weights & Biases Weave](https://wandb.ai/site/weave/)** — Tracing and evaluation for model applications, inside the experiment tracking many teams already run. `Freemium` `Web` `API`

## How agents are selected

An entry qualifies when it does two things: pursues a goal across several steps without being
re-prompted at each one, and acts on something outside the conversation through tools, code
execution, a browser, or an API.

That rules out a lot of what gets called an agent. A chat assistant with tool calling is an
assistant. A workflow builder with a fixed sequence of steps is automation. Both are useful
and neither is listed here unless the product genuinely decides what to do next.

Three kinds of thing appear, and the category says which:

- **End-user agents** are products you point at a task. Categories one to seven.
- **Platforms and frameworks** are what you build agents with. Hosted builders and code
  libraries are kept in separate categories because the audiences barely overlap.
- **Infrastructure** is what runs underneath: sandboxes, browsers, tool connectors, memory,
  evaluation, observability.

Where a project is open source, it carries the `Open Source` label, which means an
OSI-approved licence. Source-available projects with commercial restrictions do not get the
label; the description says so instead. This distinction matters more here than in most
categories, because a large share of agent tooling is source-available and marketed as open.

Entries are ordered alphabetically inside each category. Position carries no meaning, and
there is no paid placement, sponsorship, or affiliate link anywhere in this repository.

## Suggest an agent

- [Suggest an agent](../../issues/new?template=suggest-an-agent.yml)
- [Report a broken link](../../issues/new?template=report-a-broken-link.yml)

The most useful thing you can report here is a project that has stopped being maintained.
Agent tooling goes stale faster than almost anything else on GitHub, and a list that does not
prune is worse than no list.

If you built the project you are suggesting, say so in the form. It will not count against
the submission.

## Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md) for the entry format and what gets declined. The one
rule worth repeating: if it does not take multiple steps on its own, it is not an agent, and
the submission will be declined however good the product is.

## Disclaimer

Everything listed is built and operated by a third party, not by TiorAI. Agent tooling moves
unusually fast, and projects here may be renamed, absorbed, or abandoned between reviews.
Licences change too, so check the current licence before you build on anything labelled
`Open Source`. Listing here is editorial selection, not endorsement.

Agents that execute code or drive a browser act with whatever permissions you give them.
Nothing in this list has been audited for safety, and the usual precautions apply.

## License

[CC BY 4.0](LICENSE). You may copy, adapt, and redistribute this list, including
commercially, as long as you credit TiorAI and indicate what you changed.

The licence covers the curation, the categories, and the descriptions. It does not cover the
TiorAI name and logo, and it does not cover the linked projects, their trademarks, or their
code, which carry their own licences.

## About TiorAI

[TiorAI](https://tiorai.com/) is an AI tools directory covering far more products than this
list does, with profiles, comparisons, and alternatives pages.

This repository is the agent-shaped slice of it, and the only one in the portfolio that
covers developer frameworks and infrastructure alongside finished products.

- [AI tools directory](https://tiorai.com/tools/)
- [Automation and workflow tools](https://tiorai.com/tool-category/automation-workflows/)
