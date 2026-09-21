# Technical handoff

## Existing operator work
Repository: https://github.com/TumeloRamaphosa/Portable-agents
Branch: codex/agent-operator-onboarding
Commit recorded in this conversation: e57ecf4.

The preceding work added an offline onboarding page, nine labelled integration candidates, browser-local task storage and JSON export. This is not live agent dispatch. Keep shared operator code there; this repository contains the Bitfury project so the projects can evolve without duplicate codebases.

## Proposed components
- OpenClaw Command Center: https://github.com/jontsai/openclaw-command-center — candidate monitoring dashboard. Its reviewed README lists multi-agent orchestration as future work; Hermes/MCP interoperability is not established.
- OpenClaw and Hermes adapters: authenticate agents, discover capabilities, dispatch task IDs and return progress plus deliverable links. Not implemented here.
- MCP bridge: controlled tool access with project-scoped credentials. Exact bridge implementation remains to be selected and verified.
- Needle: https://github.com/cactus-compute/needle — candidate local tool selection/extraction/embedding model. Not installed or benchmarked for Studex. Requires application adapters and permission checks; does not provide Drive sync or full orchestration.
- Obsidian: editable local Markdown knowledge.
- Google Drive: proposed project-scoped inputs and deliverables; destination and access must be established before private documents are uploaded.
- ClickUp: task ownership and progress; Notion: project knowledge and decisions.

## Initial acceptance test
1. Connect one authenticated OpenClaw agent and one Hermes agent.
2. Give each an approved, non-sensitive sample document.
3. Dispatch a summarisation task with a unique ID and output location.
4. Check actual execution, saved output, provenance and task status update.
5. Test disconnected state, retries and duplicate prevention.

Local work should use cached approved files and a durable queue. Remote tools still need connectivity. Preserve versions and flag conflicting edits when synchronising. Do not mark agents online without a current authenticated health check.

## Known limitations from this task
No live VM connection, MCP dispatch, RAG index or Drive synchronisation has been completed here. Notion agent execution previously returned a missing 'interact with agents' permission. Historical fleet counts and VM alerts supplied in chat are not current health evidence.

No credentials, private correspondence, phone numbers, contracts or whole-vault exports belong in this public repository. Meeting recording requires participant notice and applicable consent.
