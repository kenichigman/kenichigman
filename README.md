### I build agent systems and the infrastructure they run on.

Cybersecurity student. I care about protection: of people, of agents, and
of the shared spaces they work in. Most of what I build runs unattended,
so it has to be honest about what it did and why.

**Nightwatch** — [an agentic framework](https://github.com/kenichigman/nightwatch-code)
for building calibrated, falsifiable agent systems. A cloud agent head
holds the judgment. Specialist agents do bounded work in parallel and
return fixed-size outputs. Every claim gets scored against the outcome.
Rules are pre-registered as code, so the system argues through
falsification, not discretion. The reference build is a prediction-market
research engine: quarter-Kelly sizing, mechanical EV gates, Brier-score
calibration, kill conditions on the doctrines themselves.

**The execution tier** — the framework runs a second tier on a
workstation I own: local LLM inference and a small fleet of cloned VMs
for parallel data collection. It wakes on demand under reference-counted
leases, sleeps when nobody needs it, and never holds credentials or a
commit path. If it goes dark, the work gets slower. It does not get
wronger. Design notes are in the repo
([execution-tier.md](https://github.com/kenichigman/nightwatch-code/blob/main/docs/execution-tier.md)).

**Other builds**

- A collectibles pipeline: inventory classification and pricing for a
  high-volume resale operation, Python + SQLite + local LLMs.
- An [audio-driven music-video engine](https://github.com/kenichigman/music-video):
  real audio features drive every frame. No procedural stand-ins.

**Stack:** Python, C++, SQLite, Next.js, local inference (Ollama),
VM fleets, multi-agent orchestration.
