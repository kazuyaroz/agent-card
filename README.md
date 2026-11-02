# agent-card

An [A2A](https://agent-to-agent.dev) **agent card** — the machine-readable capability document an agent publishes so other agents can discover what it does, how to reach it, and what it will accept.

Served at the conventional well-known path so any A2A-aware client can find it without prior configuration:

```
https://<host>/.well-known/agent-card.json
```

## What's in it

- **Identity** — agent name, description, and the public key it signs with
- **Capabilities** — the operations the agent exposes, with input/output schemas
- **Endpoints** — where to call each capability
- **Payment terms** — accepted assets, chains and pricing, where the agent charges for work

## Why it exists

Agent-to-agent discovery is the boring half of multi-agent systems and the part everyone reinvents. A card at a fixed, well-known path means a new agent can be integrated by pointing a client at a URL — no registry, no allowlist, no out-of-band setup.

## Related

- [`portfolio`](https://github.com/kazuyaroz/portfolio) — security research portfolio, also publishes an agent card
- [`bounty-hunter`](https://github.com/kazuyaroz/bounty-hunter) — multi-platform bounty automation that consumes agent marketplaces

---

*Part of my security research work — see the [portfolio](https://kazuyaroz.github.io/portfolio).*
