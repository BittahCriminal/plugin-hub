# Plugin Hub

Marketplace for ByteCloud Claude Code plugins. Each plugin lives in its own
repo; this hub just lists them, so users add one marketplace and can install
any of them.

```
/plugin marketplace add BittahCriminal/plugin-hub
/plugin install chief-of-staff
```

## Listed plugins

| Plugin | Repo | What it is |
|---|---|---|
| chief-of-staff | [BittahCriminal/Chief-of-Staff](https://github.com/BittahCriminal/Chief-of-Staff) | Career operating skills, voice-matched comms, design review personas, read-only briefing harness |
| platform-engineering | [BittahCriminal/platform-engineering-plugin](https://github.com/BittahCriminal/platform-engineering-plugin) | Kubernetes ops, GitOps/CI-CD, IaC, observability, platform design (scaffold) |
| career-advancement | [BittahCriminal/career-advancement](https://github.com/BittahCriminal/career-advancement) | Promotion positioning, visibility, level-up behaviors, feedback, negotiation (scaffold) |
| volcano-scheduling | [BittahCriminal/volcano-scheduling-plugin](https://github.com/BittahCriminal/volcano-scheduling-plugin) | Offline-first Volcano batch scheduling for Kubernetes: queues, PodGroups, VolcanoJob, scheduler actions/plugins, GPU/vGPU sharing, network-topology-aware scheduling |
| rag-mcp | [BittahCriminal/rag-mcp-plugin](https://github.com/BittahCriminal/rag-mcp-plugin) | Read-only semantic search over the ByteCloud technical library (29 books, 384 chapter transcripts, platform engineering reports) via Qdrant; Cloudflare Access service-token auth |
| swe | [BittahCriminal/SWE](https://github.com/BittahCriminal/SWE) | Dependency-free Go runtime for smallest-correct-change engineering guidance |

## Adding a plugin

Append an entry to `.claude-plugin/marketplace.json` with a
`{"source": "github", "repo": "owner/repo"}` source. The plugin repo needs
its own `.claude-plugin/plugin.json`. Version, release, and issues stay in
the plugin's repo — the hub only carries the listing.
