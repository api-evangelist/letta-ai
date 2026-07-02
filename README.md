# Letta (letta-ai)

Letta (formerly MemGPT) builds stateful AI agents with persistent memory that runs as a service. The Letta REST API creates, configures, and messages agents whose memory - core context blocks and archival vector memory - survives across sessions, and manages the tools, data sources, identities, and multi-agent groups those agents use. It is offered as a managed Letta Cloud API and as an open-source, self-hostable server with the same OpenAPI-documented interface.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/letta-ai/refs/heads/main/apis.yml)

## Tags

- AI
- Agents
- LLM
- Memory
- Stateful Agents
- MemGPT

## Timestamps

- **Created:** 2026-07-02
- **Modified:** 2026-07-02

## APIs

### Letta Agents API

Create, list, search, count, retrieve, modify, delete, import, and export stateful agents - each with its own persistent memory, tools, sources, and model configuration. Agents can be recompiled, reset, and exported as portable agent files.

- **Human URL:** [https://docs.letta.com/api-reference/agents/list](https://docs.letta.com/api-reference/agents/list)
- **Base URL:** `https://api.letta.com/v1`

#### Tags

- Agents
- Stateful Agents
- Lifecycle

#### Properties

- [Documentation](https://docs.letta.com/guides/core-concepts/stateful-agents/)
- [API Reference](https://docs.letta.com/api-reference/agents/list)
- [OpenAPI](openapi/letta-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Letta Messages API

Send synchronous, asynchronous, and streaming messages to an agent, list and search message history, cancel an in-flight run, preview the raw model payload, and reset or summarize an agent's conversation. Streaming is delivered as Server-Sent Events over the messages/stream endpoint.

- **Human URL:** [https://docs.letta.com/api-reference/agents/messages/stream](https://docs.letta.com/api-reference/agents/messages/stream)
- **Base URL:** `https://api.letta.com/v1`

#### Tags

- Messages
- Streaming
- Conversations

#### Properties

- [Documentation](https://docs.letta.com/guides/core-concepts/messages/streaming/)
- [API Reference](https://docs.letta.com/api-reference/agents/messages/create)
- [OpenAPI](openapi/letta-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/letta-ai-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### Letta Memory Blocks API

Manage core-memory blocks - the labeled, always-in-context text that gives an agent its persona, human, and task memory. Create, list, retrieve, modify, and delete standalone blocks, and attach or detach blocks to and from agents, groups, and identities to share memory across them.

- **Human URL:** [https://docs.letta.com/guides/core-concepts/memory/memory-blocks/](https://docs.letta.com/guides/core-concepts/memory/memory-blocks/)
- **Base URL:** `https://api.letta.com/v1`

#### Tags

- Memory
- Core Memory
- Blocks

#### Properties

- [Documentation](https://docs.letta.com/guides/core-concepts/memory/memory-blocks/)
- [API Reference](https://docs.letta.com/api-reference/blocks/list)
- [OpenAPI](openapi/letta-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Letta Archival Memory API

Manage archives - an agent's out-of-context, searchable long-term memory - and the passages stored inside them. Create and list archives, attach or detach an archive to an agent, and create, batch-create, search, and delete individual archival passages.

- **Human URL:** [https://docs.letta.com/api-reference/archives/list-archives](https://docs.letta.com/api-reference/archives/list-archives)
- **Base URL:** `https://api.letta.com/v1`

#### Tags

- Archival Memory
- Archives
- Passages
- Vector Search

#### Properties

- [Documentation](https://docs.letta.com/guides/core-concepts/memory/archival-memory/)
- [API Reference](https://docs.letta.com/api-reference/archives/list-archives)
- [OpenAPI](openapi/letta-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Letta Tools API

Create, list, search, count, upsert, modify, delete, and directly run tools (Python functions) that agents call. Includes registering the built-in base tool set and executing a tool from raw source without attaching it to an agent first.

- **Human URL:** [https://docs.letta.com/api-reference/tools/list](https://docs.letta.com/api-reference/tools/list)
- **Base URL:** `https://api.letta.com/v1`

#### Tags

- Tools
- Function Calling
- Sandbox

#### Properties

- [Documentation](https://docs.letta.com/guides/core-concepts/tools/server-tools/)
- [API Reference](https://docs.letta.com/api-reference/tools/list)
- [OpenAPI](openapi/letta-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Letta MCP Servers API

Register, connect, test, refresh, update, and delete remote MCP (Model Context Protocol) servers, list the tools each server exposes, add an individual MCP tool to an agent's toolset, and execute an MCP tool directly, including OAuth-based MCP server connections.

- **Human URL:** [https://docs.letta.com/api-reference/tools/list-mcp-servers](https://docs.letta.com/api-reference/tools/list-mcp-servers)
- **Base URL:** `https://api.letta.com/v1`

#### Tags

- MCP
- Model Context Protocol
- Tool Servers

#### Properties

- [Documentation](https://docs.letta.com/guides/core-concepts/tools/mcp-tools/)
- [API Reference](https://docs.letta.com/api-reference/tools/list-mcp-servers)
- [OpenAPI](openapi/letta-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Letta Sources and Files API

Create and manage data sources (also exposed as folders) that hold uploaded files for agent grounding and retrieval - upload files, list and delete files and their extracted passages, and attach or detach a source to an agent's file system.

- **Human URL:** [https://docs.letta.com/api-reference/sources/list](https://docs.letta.com/api-reference/sources/list)
- **Base URL:** `https://api.letta.com/v1`

#### Tags

- Sources
- Folders
- Files
- RAG

#### Properties

- [Documentation](https://docs.letta.com/guides/core-concepts/filesystem/)
- [API Reference](https://docs.letta.com/api-reference/sources/list)
- [OpenAPI](openapi/letta-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Letta Identities API

Model the end users of a multi-tenant Letta deployment as identities. Create, list, count, retrieve, modify, upsert, and delete identities; set custom identity properties; and attach or detach an identity to agents and memory blocks so many agents can share one user's context.

- **Human URL:** [https://docs.letta.com/api-reference/agents/identities/attach](https://docs.letta.com/api-reference/agents/identities/attach)
- **Base URL:** `https://api.letta.com/v1`

#### Tags

- Identities
- Multi-Tenant
- End Users

#### Properties

- [API Reference](https://docs.letta.com/api-reference/agents/identities/attach)
- [OpenAPI](openapi/letta-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Letta Multi-Agent Groups API

Create, list, retrieve, modify, and delete multi-agent groups that coordinate several agents (round-robin, supervisor, and other patterns) around shared memory blocks. Attach or detach shared blocks, and list, modify, and reset the group's combined message history.

- **Human URL:** [https://docs.letta.com/guides/core-concepts/memory/shared-memory/](https://docs.letta.com/guides/core-concepts/memory/shared-memory/)
- **Base URL:** `https://api.letta.com/v1`

#### Tags

- Groups
- Multi-Agent
- Shared Memory

#### Properties

- [Documentation](https://docs.letta.com/guides/core-concepts/memory/shared-memory/)
- [API Reference](https://raw.githubusercontent.com/letta-ai/letta/main/fern/openapi.json)
- [OpenAPI](openapi/letta-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Letta Models and Providers API

List available LLM and embedding models, and register, check, list, retrieve, modify, delete, and refresh bring-your-own-key (BYOK) model providers (OpenAI, Anthropic, Google, Azure, local/self-hosted, and more) that agents can be configured to use.

- **Human URL:** [https://docs.letta.com/api-reference/models/list](https://docs.letta.com/api-reference/models/list)
- **Base URL:** `https://api.letta.com/v1`

#### Tags

- Models
- Providers
- BYOK

#### Properties

- [Documentation](https://docs.letta.com/guides/build-with-letta/models/)
- [API Reference](https://docs.letta.com/api-reference/models/list)
- [OpenAPI](openapi/letta-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Letta Runs, Jobs and Steps API

Inspect the asynchronous execution history behind agent messages. List and retrieve runs and their messages, metrics, usage, trace, and stream; list and cancel background jobs; and list steps (individual model calls within a run) with per-step feedback, metrics, and trace.

- **Human URL:** [https://docs.letta.com/api-reference/runs/list](https://docs.letta.com/api-reference/runs/list)
- **Base URL:** `https://api.letta.com/v1`

#### Tags

- Runs
- Jobs
- Steps
- Observability

#### Properties

- [Documentation](https://docs.letta.com/guides/observability/monitoring)
- [API Reference](https://docs.letta.com/api-reference/runs/list)
- [API Reference](https://docs.letta.com/api-reference/jobs/list)
- [OpenAPI](openapi/letta-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Letta Agent Templates API

Cloud-only API for versioning agent configurations as templates - create, save, roll back, rename, and delete template versions, snapshot and restore a template from an agent file, and deploy new agents from a template version.

- **Human URL:** [https://docs.letta.com/guides/templates/client-side-tokens/](https://docs.letta.com/guides/templates/client-side-tokens/)
- **Base URL:** `https://api.letta.com/v1`

#### Tags

- Templates
- Deployments
- Cloud Only

#### Properties

- [Documentation](https://docs.letta.com/guides/templates/client-side-tokens/)
- [API Reference](https://raw.githubusercontent.com/letta-ai/letta/main/fern/openapi.json)
- [OpenAPI](openapi/letta-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Letta Chat Completions API

OpenAI-compatible chat completions endpoint that routes requests to a Letta agent, plus a companion voice-beta chat completions endpoint tuned for low-latency voice agent integrations.

- **Human URL:** [https://docs.letta.com/guides/get-started/intro](https://docs.letta.com/guides/get-started/intro)
- **Base URL:** `https://api.letta.com/v1`

#### Tags

- Chat Completions
- OpenAI Compatible

#### Properties

- [API Reference](https://raw.githubusercontent.com/letta-ai/letta/main/fern/openapi.json)
- [OpenAPI](openapi/letta-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/letta-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/letta-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/letta-ai)
- [LinkedIn](https://www.linkedin.com/company/letta-ai)
- [Website](https://www.letta.com)
- [Documentation](https://docs.letta.com)
- [Plans](plans/letta-ai-plans-pricing.yml)
- [Rate Limits](rate-limits/letta-ai-rate-limits.yml)
- [Fin Ops](finops/letta-ai-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
