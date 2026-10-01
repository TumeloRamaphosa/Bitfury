# Partners & Infrastructure Registry

**Last Updated:** 2026-09-28  
**Owner:** Tumelo Ramaphosa  
**Goal:** 24/7 agent operations across 5+ countries + partner ecosystem

---

## Partner VM Deployments

| Partner | Territory | VM Provider | Instance Type | Status | Agent Workload | Owner |
|---------|-----------|-------------|---------------|--------|----------------|-------|
| **Bitfury** | Rwanda + Regional | Lake Kivu Power (Proposed) | Compute Optimized | Pre-contract | Infrastructure POC | Vadim / Tumelo |
| **UNDP Timbuktoo** | Rwanda | TBD (Diligence) | Standard | Proposed | AI + Gaming Hub | Tumelo |
| **Studex Meat** | SA + Eswatini | Railway | 2x Standard | ✅ Live | Naledi CMO + EDDIE Ad Engine | Charlie (Voice) |
| **Studex Global Markets** | SA + Rwanda | Vercel (Edge) | Serverless | ✅ Live | RALF Loop + OpenClaw | Adam Smasher |
| **Black Cloud OS** | Local + SA | Local (Mac Mini M4) | 16GB RAM | ✅ Live | Hermes Orchestrator + Full stack | Tumelo |
| **Naledi Nexus** | WhatsApp + Social | Vercel + n8n | Serverless + Workflow | ✅ Live | 9 autonomous agents | RALF |
| **Adam Labs** | Ubuntu 22.04 | Hetzner | 2x RTX 4090 (planned) | Sourced | Research + AI training | Adam Smasher |
| **Pharma Ops** (Bunny-Rabbit) | SA + Eswatini + Rwanda | TBD (Bunny Lead) | Multi-zone | Proposed | Supply chain + Manufacturing | Katlego / Tumelo |

---

## Planned Expansion (Oct 31 — Dual Hub Launch)

### Cape Town Hub (18:00 SAST)
- **Partner:** Bitfury (Bitcoin Trust genesis)
- **Infrastructure:** Local colocation + Vercel CDN
- **Agents:** Market Scout, Investment Hunter, Fundraiser
- **Data:** 37K+ commodities, live trading engine
- **Status:** Venue + partnership contracts in progress

### Kigali Hub (14:00 EAT)
- **Partner:** UNDP + Rwanda Government
- **Infrastructure:** Lake Kivu power grid + local ISP
- **Agents:** Naledi (CMO) + Charlie (Voice intake) + EDDIE (Ad spend)
- **Data:** Agricultural commodities, regional markets
- **Status:** Diligence phase (power capacity, permits)

---

## Active Agent Deployments

### Tier 1: Always-On (24/7)
| Agent | Model | Infrastructure | Cadence | Owner | Status |
|-------|-------|-----------------|---------|-------|--------|
| **Hermes** | Node.js orchestrator | Black Cloud (:3000) | Always | Tumelo | ✅ Running |
| **Kev** | 4B decision router | Local (Ollama :8009) | Always | Tumelo | ✅ Running |
| **RALF** | DeepSeek-R1 loop | n8n + Vercel | Midnight + 6h checks | Tumelo | ✅ Scheduled |
| **Blotato** | Multi-platform poster | API endpoint | On-demand | Naledi → Kev | ✅ Ready |

### Tier 2: Scheduled (Key Cadences)
| Agent | Cadence | Launch Time | Owner | Status |
|-------|---------|-------------|-------|--------|
| **Naledi** | Daily (06:00 SAST) | 2026-09-29 | Tumelo | ✅ Ready |
| **EDDIE** | Every 4 hours | Async loop | Tumelo | ✅ Ready |
| **Charlie** | On incoming call | Twilio trigger | Katlego | ✅ Ready |
| **Market Scout** | Daily morning brief | 07:00 SAST | Tumelo | ⏳ Wired to Hermes |

### Tier 3: Pre-Deployment (Bitfury / Rwanda)
| Agent | Role | Deployment Target | Dependencies | ETA |
|-------|------|-------------------|--------------|-----|
| **Investment Hunter** | Revenue opportunity scanner | Global Markets API | Bitfury partnership, Hermes bridge | Oct 15 |
| **Fundraiser** | Automated cap table + investor outreach | Black Cloud + Gmail | AgentMail wiring, LiteLLM router | Oct 15 |
| **Regional CMO** | Rwanda market content | Kigali Hub + Blotato | Lake Kivu infra live | Nov 1 |

---

## Agent Command Architecture (24/7 Loop)

```
Hermes Orchestrator (Black Cloud :3000)
├── Kev (Decision router)
│   ├── Route to Naledi (content)
│   ├── Route to EDDIE (spend)
│   └── Route to Charlie (voice)
├── RALF (Midnight coordinator)
│   ├── Sync all agent outputs
│   ├── Update Obsidian vault
│   └── Queue tomorrow's tasks
└── OpenWorker (Job queue :7000)
    ├── 8 worker pool
    ├── Auto-retry failed tasks
    └── Report to Notion dashboard
```

---

## Integration Checklist (48-Hour Sprint)

- [ ] **Partner Listings Live** — Global Markets + Black Cloud sites show all 8 partners + VM status
- [ ] **Agent Status Dashboard** — Artifact shows Tier 1 agents (24/7), Tier 2 (scheduled), Tier 3 (pending)
- [ ] **VM Health Monitor** — Real-time CPU/memory from each deployment (railway, vercel, hetzner, local)
- [ ] **Agent Command Center** — Dispatch tasks to Hermes, see live execution + provenance
- [ ] **Loop Goal Automation** — RALF sync every 6h, Notion + Obsidian + Notion updates
- [ ] **Bitfury Agent Bridge** — Once partnership signed, auto-register new agents to Hermes
- [ ] **Rwanda Pilot Ready** — Charlie voice + Naledi content staging for Oct 1 delegation

---

## Revenue Tracking (Agent-Driven)

| Source | Agent Owner | Status | Oct 30 Target | Nov 30 Target |
|--------|------------|--------|---------------|---------------|
| Meat store (WhatsApp) | Charlie + RALF | ✅ Live | $8K | $15K |
| Ad spend (EDDIE ROAS) | EDDIE + Kev | ✅ Live | $12K | $25K |
| Trading signals (Market Scout) | Market Scout | ⏳ Launching | — | $10K |
| Fundraising (Investment Hunter) | Investment Hunter | ⏳ Wired to Hermes | — | Closed $500K |

---

## Next Immediate Actions

1. **Today (Sep 28):** Finalize Bitfury NDA, confirm speaker + Rwanda meetings
2. **Tomorrow (Sep 29):** Launch Naledi + RALF on schedule, test Hermes → Tier 2 routing
3. **Oct 1–5:** Rwanda delegation (sync partner learnings back to Hermes)
4. **Oct 15:** Investment Hunter + Fundraiser live on Global Markets
5. **Oct 31:** Dual Hub launch (Cape Town 18:00 + Kigali 14:00)
