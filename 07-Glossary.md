
```markdown
# AI Agent Systems Engineering: Encyclopedia-Style Technical Glossary

This technical glossary serves as a comprehensive reference guide for the core terms, design patterns, security frameworks, and software protocols covered during the 5-Day Intensive AI Agents and Vibe Coding curriculum. The concepts below are organized alphabetically and explained using professional system engineering language.

---

## Key Architectural Formulas

To establish quick structural alignments before diving into individual terms, keep these foundational software formulas in mind:

$$\text{Agent} = \text{Model} + \text{Harness}$$

$$\text{Harness} = \text{Memory} + \text{Tools} + \text{Runtime} + \text{Governance}$$

$$\text{Model Context Protocol (MCP)} = \text{Standardized Transport Interface Layer}$$

$$\text{Agent Skill Pack} = \text{Decoupled Procedural Memory File Map}$$

---

# A

### ADK (Agent Development Kit)
An open-source software development kit engineered by Google to build, instrument, evaluate, and scale autonomous AI systems. Moving past basic text completion interfaces, the ADK provides standard classes and decorators to map multi-node workflow graphs, register executable tools, enforce runtime context constraints, and insert out-of-band Human-in-the-Loop approval checkpoints.

### Agent
An autonomous software system that wraps an underlying foundational language model inside a stateful execution harness. Unlike classic request-response chatbot pipelines that execute simple text transformations ($\text{Inference}(X) \rightarrow Y$), an agent uses an active loop to independently observe environment parameters, formulate multi-step execution plans, call external tools, handle system errors, and modify real-world states over time.

### Agentic Engineering
The specialized discipline of designing, constructing, and hardening software systems that delegate task orchestration and execution paths to autonomous AI planners. Its primary focus is building the structural boundaries—such as isolated tool registries, validation filters, evaluation pipelines, and fallback states—needed to make non-deterministic model actions reliable enough for enterprise applications.

### Agents CLI
An advanced command-line interface utility engineered to manage the complete lifecycle of agentic software assets. It provides development teams with terminal-based commands to scaffold clean project directories, validate skill configurations, compile runtime traces, run automated regression datasets, and deploy containerized agent nodes directly to cloud environments.

### Ambient Agent
An event-driven, background software agent that executes planning loops and modifies system states automatically when triggered by environment alerts, cron schedules, or platform message buses. Unlike standard conversational chatbots, ambient agents run without a direct user watching or managing the active terminal session.

### Antigravity
Google's agent-native Integrated Development Environment (IDE) engineered to optimize Vibe Coding workflows. It provides native Model Context Protocol (MCP) clients, live visualization layers for active agent workflows, built-in tool sandboxes, automated security linting hooks, and real-time context management systems.

---

# C

### Context
The complete token payload populated into a transformer's active attention window during a single inference cycle. It acts as the agent's absolute working memory for that explicit execution step, and is typically structured to hold core system prompts, historical session logs, active database schemas, tool returns, and the user's input string.

### Context Engineering
The disciplined process of structuring, updating, and optimizing the token payload entering a model's context window. By using explicit markers (like XML tags), stripping out repetitive logs, and caching static parameters, context engineering improves reasoning focus, drops response latency, eliminates hallucinated paths, and cuts API token spend.

### Context Rot
The severe degradation of an agent's planning logic and instruction adherence that happens when unmanaged historical logs clutter the context window. As tokens scale, the attention mechanism dilutes, causing the model to forget core boundaries, invent tool arguments, or fall into infinite execution loops (the "lost-in-the-middle" trap).

### Cloud Run
Google Cloud's fully managed, serverless container platform used to host and scale production agent applications. It runs containerized agent nodes inside isolated enclaves, automatically scaling instances based on incoming event traffic and separating secrets handling from the underlying model logic.

---

# D

### Dynamic Context
Data hydrated into an agent's context window on demand based on specific events triggered during the active loop. Rather than front-loading massive datasets into the initial prompt, dynamic context uses vector searches (RAG), database lookups, or API calls to inject precise information snippets only when the planner needs them.

---

# E

### Evaluation (Eval Pipelines)
The systematic process of measuring, grading, and tracking the safety and accuracy of non-deterministic agent trajectories over standardized test datasets. Unlike traditional software test arrays, agent evaluation pipelines grade system outputs across qualitative metrics like instruction alignment, safety policy compliance, and tool loop efficiency.

### Event-Driven Architecture
A software design topology where actions and computations are triggered in response to state shifts, webhooks, file writes, or system messages. It serves as the core infrastructure layout for deploying ambient agents, connecting message brokers (like Cloud Pub/Sub) directly to ephemeral agent execution runtimes.

---

# G

### Gemini
Google's family of highly advanced, multi-modal foundational models. Engineered with native support for function calling, structured JSON output generation, complex reasoning, and long context windows, Gemini serves as the core cognitive processing unit for enterprise agent systems.

### Gherkin
A line-oriented, machine-readable behavior specification language that utilizes an explicit `Given-When-Then` framework to define software features. In Spec-Driven Development, Gherkin acts as the immutable source of truth, establishing clear behavioral requirements that humans read and code generation agents implement.

---

# H

### Human-in-the-Loop (HITL)
A critical governance checkpoint pattern that inserts an out-of-band human manual approval stage into an autonomous workflow. The system state is completely paused before high-risk tools fire—such as initiating wire transfers or deleting database tables—demanding an authorized administrative sign-off before execution can resume.

---

# L

### LLM-as-a-Judge
An automated evaluation design pattern that leverages an independent, highly capable reasoning model to review and grade an agent's complete execution trace. The judging model analyzes the interaction history against a strict, structured rubric, returning a numerical score alongside an explicit justification log.

---

# M

### Memory
The core architectural layer that allows an agent system to retain, organize, and recall state information across distinct processing loops and user sessions. It is divided into three distinct functional topologies:
* **Short-Term Memory:** Tracks the immediate conversational context and current step logs within the active window.
* **Long-Term Memory:** Uses external vector databases to recall patterns and data structures from past execution histories.
* **Procedural Memory:** Uses modular skill directories to store step-by-step expertise detailing *how* to perform specific engineering tasks.

### MCP (Model Context Protocol)
An open-standard, asymmetrical application-layer protocol designed to establish uniform communication between AI reasoning clients and external tools, databases, and application spaces. Operating over JSON-RPC 2.0 frameworks, it abstracts capabilities away from custom integration script layers, acting as the universal adapter for agent tools.

### MCP Client
The host integration engine that runs inside an agent application or workspace (like Google Antigravity). It orchestrates connections to active servers, maps available capabilities to the model, and packages raw tool responses into protocol-compliant text layers.

### MCP Server
An independent process or microservice that securely exposes Tools, Resources, and Prompts to connected clients. It manages infrastructure tokens locally at the data source and runs all execution commands inside secure enclaves, completely isolated from model planning risks.

---

# O

### OpenTelemetry
An open-source observability framework used to capture, export, and analyze system traces, execution logs, and performance metrics across distributed software ecosystems. In agent engineering, it tracks complete execution paths, showing every step from initial prompt to internal tool call.

---

# P

### Policy Server
A centralized, isolated authorization gatekeeper that sits directly between the agent runtime and production infrastructure. It monitors every tool request generated by the model and validates parameters against role-based access rules and daily spend budgets to authorize or block the command before it fires.

### Prompt Injection
An adversarial attack vector where malicious, untrusted text strings manipulate a model's token prediction path, overriding the developer's system prompt constraints. This threat is native to modern architectures because system rules and raw data inputs share the same unstructured text context window.

### Procedural Memory
The cognitive layer dedicated to storing step-by-step knowledge detailing *how* to perform a complex sequence of tasks reliably over time. Within production agent platforms, procedural memory is decoupled from model weights and codified inside structured Agent Skill packs.

### Pub/Sub
An asynchronous, event-driven messaging layer that decouples services that produce events from services that process events. It handles traffic routing for ambient systems, ensuring that infrastructure alerts trigger background agent loops instantly without dropping connection states.

---

# R

### Reasoning Loop
The continuous execution chain used by autonomous agents to navigate complex goals. It follows a structured path—**Observe** current environment states, **Think** to plan immediate sub-tasks, **Act** by executing a target tool, and **Evaluate** the returned results—looping continually until the objective clears verification checks.

### Runtime
The complete system execution environment where an agentic application operates. It coordinates memory modules, manages tool access lines, traces workflow graphs, and enforces policy server guardrails across active processing sessions.

---

# S

### Skill (Agent Skill Pack)
A modular, portable capability directory that encapsulates deep behavioral prompts, operational rules, design checklists, and execution scripts for a specific domain task. It uses a master `SKILL.md` manifest to load instructions dynamically only when an active intent is matched, eliminating context rot.

### Spec-Driven Development (SDD)
A rigorous development methodology where formal, machine-readable specifications serve as the unchangeable source of truth for an application. While the specification files remain permanent records of design intent, the underlying codebase is treated as a temporary, machine-generated artifact that can be cleanly regenerated from the spec at any time.

### STRIDE
A classical threat-modeling framework used to systematically map security risks across six distinct failure vectors: **S**poofing identity, **T**ampering with data, **R**epudiation of actions, **I**nformation disclosure leaks, **D**enial of service loops, and **E**levation of privilege blocks.

---

## T

### Tool
A secure, typed interface exposed to an agent's execution harness, allowing the core language model to read or modify external environment states. Examples include database queries, repository file editors, cloud resource runners, and API clients.

### Tool Calling (Function Calling)
The process where a foundational language model consumes an abstract tool schema, evaluates its active plan against current goals, and outputs a structured JSON object specifying a target function name alongside precise argument variables.

---

# V

### Vibe Coding
A software delivery methodology where developers focus entirely on authoring, tuning, and verifying high-level system specifications and architectural boundaries in natural language, while automated generation agents handle compiling the underlying code files.

---

# W

### Workflow
A directed acyclic graph (DAG) layout that structures an agent's planning logic into explicit nodes and edges. Each node represents a specific reasoning state or tool action, while edges map the conditional state transitions that guide the system through complex tasks.

---

# Comprehensive Primitives Matrix

Use this high-speed summary matrix to quickly map the primary roles of different agent platform components:

| Framework Asset | Core Structural Role | Simple Analogy |
| :--- | :--- | :--- |
| **Foundational Model** | Linguistic vector transform & logical inference | **The Brain:** Abstract reasoning engine |
| **Agent Harness** | System state-tracking and execution environment | **The Body:** Interface shell framework |
| **MCP Specification** | Unified protocol wires over JSON-RPC 2.0 channels | **The Hardware Ports:** Standard integration wires |
| **Agent Skill Pack** | Self-contained, portable procedural expertise | **The Apps:** Plugins loaded only when needed |
| **Policy Server** | Out-of-band authorization and security gatekeeper | **The Firewall:** Strict security enforcement gate |
| **Spec-Driven Dev** | Specification-first automated application build runs | **The Master Blueprint:** Source of truth map |
| **Human-in-the-Loop** | Manual approval gate for critical commands | **The Safety Switch:** Absolute control layer |
| **Ambient Agent** | Event-driven, background orchestration engine | **The Automated Monitor:** Continuous helper tool |

---

## References and Core Standards Documents

* **Google Antigravity SDK & ADK Specifications:** System layout requirements and runtime protocols.
* **Model Context Protocol Open Source Transport Docs:** Standard schemas and message structures for JSON-RPC.
* **The Gherkin Behavioral Specification Standards:** Grammar patterns for writing clean Given-When-Then logic paths.
* **The STRIDE Security Classification Framework:** Security modeling guides for machine learning workflows.

```

---

## Visual Relationship Map
Agent
│
├── Model (Gemini)
├── Memory
├── Tools
├── Skills
├── MCP
├── Policies
└── Runtime

```

Your documentation suite is nearly complete. Let me know when you are ready to construct the final capstone module: **`08-Course-Summary.md`**!
