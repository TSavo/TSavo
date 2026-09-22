# T Savo

I build systems that build systems.

Thirty years of production software — XDrive (acquired by AOL), IFilm (acquired by
MTV), Neopets, CBS, true[X]/Fox, Tillster. The last several years have been
agent-driven development at production throughput: I design the system, a fleet
writes against it, and I own what ships.

**2,857 commits in five weeks** on a live commerce platform. **9,394 commits in five
months** on a formal verification substrate. Operating systems with real money and
real proofs behind them, not prototypes. The commit dates are public.

Available for work. Los Angeles, and I relocate. · `evilgenius@nefariousplan.com`

---

### [Sugar](https://github.com/TSavo/sugar) — proofs from the code you already wrote
`Rust` · `z3` · `BLAKE3`

Lifts unit tests, assertions and function bodies into pinned first-order logic and
emits a signed, content-addressed `.proof` — no spec language, no annotations, no
changes to your code.

`sugar diff` compares two releases by *behavior* and classifies every contract as
held, renamed, new or lost, so a "minor" release that quietly changes semantics
lights up before it reaches production. `sugar prove` hands z3 your callsite
assumption alongside the dependency's lifted contract and refuses the wrong ones
before anything runs. Rust, Python and Java lift into one shared logic, so a Rust
caller can be checked against a Python library's proven behavior at the same
callsite.

A kit never becomes the authority on what your code means — it rules only by citing
the vendor's own tests and compiler. What it can't see is reported as an effect, a
residue, or a refusal. Never painted green.

### [WOPR](https://github.com/TSavo/wopr) — self-sovereign agent runtime
`npm i -g @tsavo/wopr` · `TypeScript`

Persistent AI sessions with a plugin architecture and agent-to-agent P2P over
Ed25519/X25519 identity. Three-layer security: trust levels, capability gating, and
Docker sandbox isolation, with controlled escalation from untrusted to privileged
sessions through gateway routing. Around twenty first-party plugins spanning Discord,
Slack, Telegram, WhatsApp, Signal, iMessage and Teams, plus providers for Anthropic,
OpenAI and Kimi.

### [Malice](https://github.com/TSavo/Malice) — a text MMO engine, ten years in
`TypeScript` · `RxJS` · `MongoDB`

LambdaMOO-style prototype inheritance where game logic lives in the database as
executable methods and everything that acts is an agent. Telnet, WebSocket and TLS
client-certificate transports; an O(1) array-backed object cache behind a stable
proxy; procedural world generation; NPC agents; an LSP and a VS Code extension for
programming inside the world.

### Dead Nuts — a company its own agents operate
[deadnutstools.com](https://deadnutstools.com) · `TypeScript` · `Postgres` · `Stripe`

An eBay tool brand under a lifetime warranty, and the platform that runs it.
Double-entry ledger, purchase orders with landed-cost COGS, multi-channel listing
sync, warranty claims, bank reconciliation, period close.

The warranty is the product rather than a policy attached to one, so warranty
replacement steel and warranty postage carry accounts of their own — share them with
sold steel and the cost of the promise disappears into gross margin without the trial
balance ever moving. Roughly 400 typed tools expose the business as a surface agents
act through.

### Trading
A live 15-minute BTC market maker quoting into Kalshi, with Interactive Brokers FX
integration, tick-scale market data capture, and a replay harness that tests quoting
strategies against recorded tape rather than summaries. Earlier:
[`ocho`](https://github.com/TSavo/ocho), a Node cryptocurrency exchange with its own
matching engine (2014) · [`Hippo`](https://github.com/TSavo/Hippo), exchange recording
and playback on XChange (2015) · [`Link`](https://github.com/TSavo/Link), a
file-sharing blockchain (December 2013) ·
[`cuckoo`](https://github.com/TSavo/cuckoo), memory-bound proof-of-work (2015)

### Model Context Protocol
Shipped servers five months after the protocol was published, then built discovery
infrastructure for the ecosystem.
[printify-mcp](https://github.com/TSavo/printify-mcp) (40★) ·
[creatify-mcp](https://github.com/TSavo/creatify-mcp) (23★) ·
[Unity-MCP](https://github.com/TSavo/Unity-MCP) (7★) ·
[mcplookup.org](https://github.com/TSavo/mcplookup.org) ·
[claude-orchestration-mcp](https://github.com/TSavo/claude-orchestration-mcp)

### Also
[`spectral`](https://github.com/TSavo/spectral) — a wavelength-resolved path tracer
rendering Dark Side of the Moon through a prism ·
[`transformgpt`](https://github.com/TSavo/transformgpt) — typed extraction from LLM
output, May 2023, a month before function calling shipped ·
[`mule-game`](https://github.com/TSavo/mule-game) — Web M.U.L.E. ·
[`jouster`](https://github.com/TSavo/jouster) — a Jest reporter that files failing
tests as GitHub issues ·
[`english2number`](https://github.com/TSavo/english2number-js) (31★) ·
[`proportionate-js`](https://github.com/TSavo/proportionate-js) (12★) ·
[`GoVirtual`](https://github.com/TSavo/GoVirtual) — a VM toolkit in Go (4★)

---

**Earlier:** Principal Engineer at Tillster · Lead Engineer at true[X]/Fox, where I
built Spark ETL computing daily unique viewership across every major distribution
network, a predictive autoscaler that ended outages on critical services, and a
real-time pipeline carrying 100,000+ messages a minute · Lead Architect at CBS · Lead
Architect at ClearPath, virtualized network services deployed to 1.5M users · Lead
Architect at Neopets · Lead Architect at Music Mastermind, named primary inventor on
several patents · founder of Verse Studios, exited on acquisition · Lead Engineer at
IFilm · head of R&D at XDrive, with storage patents that went to AOL in the
acquisition.
