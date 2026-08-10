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

## Adding a plugin

Append an entry to `.claude-plugin/marketplace.json` with a
`{"source": "github", "repo": "owner/repo"}` source. The plugin repo needs
its own `.claude-plugin/plugin.json`. Version, release, and issues stay in
the plugin's repo — the hub only carries the listing.
