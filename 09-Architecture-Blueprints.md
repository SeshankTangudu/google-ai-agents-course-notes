
# Comprehensive System Architecture Blueprints

This module maps out the underlying software topologies, data flows, and security boundaries explored across each day of the 5-Day AI Agents course.

---

## Day 1: The Core Model-Harness Split & Context Flows
This diagram details how the core reasoning model is decoupled from operational system utilities using an isolated application harness.

```mermaid
graph TD
    User([User Intent Input]) --> PreG[Pre-Processing Security Gateway]
    PreG -->|Sanitized Tokens| Agent[Core Agent Runtime]
    
    subgraph Harness [The Agent Harness Enclave]
        Agent <--> planning[Reasoning & Planning Loop]
        Agent <--> memory[Short-Term Session Memory]
        Agent <--> skills[Dynamic Skills Hydrator]
    end
    
    Agent -->|JSON-RPC Call| MCPClient[MCP Client Broker]
    MCPClient --> Final[Secure Tool Execution Sandbox]

```

---

## Day 2: The Model Context Protocol (MCP) Integration Layer

This sequence diagram tracks the asymmetrical client-server message transport layers navigating JSON-RPC protocol interfaces to eliminate custom integration glue code.

```mermaid
sequenceDiagram
    autonumber
    participant Agent as Core Agent Runtime
    participant Client as Local MCP Client
    participant Server as Isolated MCP Server
    participant Resource as Target API / DB Sandbox

    Agent->>Client: Identifies goal & requests data tool
    Client->>Server: Issues jsonrpc: "2.0", method: "tools/call"
    Note over Server: Validates arguments against strict JSON Schema
    Server->>Resource: Executes secure local action script
    Resource-->>Server: Returns raw execution stdout/JSON
    Server-->>Client: Packages data into standard protocol response
    Client-->>Agent: Hydrates dynamic context window with clean text

```

---

## Day 3: Dynamic Skill Packs & Progressive Disclosure

This blueprint details how massive system prompts are avoided by organizing operational behaviors into modular directories, loading explicit procedures only on demand.

```mermaid
graph TD
    Intent[User Intent Match] --> Engine{Router Script}
    Engine -->|Matches Dev Rule| SkillA[Load asset/skills/dev-scaffolder/SKILL.md]
    Engine -->|Matches Audit Rule| SkillB[Load asset/skills/code-auditor/SKILL.md]
    
    subgraph ContextWindow [Active Context Window]
        SkillA --> |Hydrate Only Active Procedure| ActiveCtx[Lightweight Context Workspace]
    end
    
    ActiveCtx --> |Prevents Context Rot| Execution[High-Performance Run]

```

---

## Day 4: Threat Modeling, PII Sanitization, & Evaluation Trajectories

This architecture maps the defensive perimeter (STRIDE parameters) alongside the automated target verification pipeline using advanced models as metrics judges.

```mermaid
graph TD
    In[Raw Payload] --> PII[PII Redaction: Aadhaar/SSN Scrubbed]
    PII --> Injection{Injection Filter}
    Injection -->|Malicious Override Blocked| Drop[Terminate Session]
    Injection -->|Safe Request Passed| Loop[Agent Planning Loop]
    Loop --> ExecutionTrace[Compile JSON Execution Trace]
    ExecutionTrace --> Judge[LLM-as-a-Judge Evaluation Enclave]
    Judge -->|Score Matrix: Latency/Safety/Cost| Dashboard[Production Analytics Dashboard]

```

---

## Day 5: Spec-Driven Development (SDD) & Policy Firewalls

This diagram traces how structural Gherkin criteria govern disposable code deployments while an isolated Policy Server authorizes or blocks live infrastructure execution.

```mermaid
graph LR
    Spec[Gherkin Feature Specs] -->|Immutable Truth| Codegen(AI Generation Agent)
    Codegen -->|Temporary Asset| Code[Disposable Codebase]
    Code --> Test[Unit Test Sandbox]
    Test --> Firewall{Policy Server Gate}
    Firewall -->|RBAC / Budget Check Passes| Deploy[Google Cloud Run Deployment]
    Firewall -->|Rule Violation Flagged| Block[Block Live Execution]
    
    style Spec fill:#1a5f7a,stroke:#333,stroke-width:2px,color:#fff
    style Code fill:#f4511e,stroke:#333,stroke-width:1px,color:#fff
    style Deploy fill:#2e7d32,stroke:#333,stroke-width:2px,color:#fff

```

```
