# Claudeforce Microsites — Project Overview

---

## Live URLs

| Site | URL |
|---|---|
| **Internal AE Battlecard** | https://edalton122.github.io/claudeforce-explainer/ |
| **External Public Explainer** | https://edalton122.github.io/claudeforce-explainer/external.html |
| **GitHub Repo** | https://github.com/edalton122/claudeforce-explainer |

---

## Site 1: Internal AE Battlecard (`index.html`)

**Audience:** Salesforce Account Executives — Internal Use Only

**Design:** Dark-mode enterprise tech style
- Background: `#0F172A` · Cards: `#1E293B`
- Salesforce Blue: `#0176D3` · Anthropic Terracotta: `#DA7756` · Success Green: `#22C55E`

### Sections

| # | Section | Key Content |
|---|---|---|
| 1 | **Hero** | "Claudeforce & AIforce AE Battlecard" — Defeating the Copilot objection, Dreamforce 2026 badge |
| 2 | **Architecture Breakdown** | 3 expandable cards: AIforce Interface Layer, Salesforce in Claude (Beta), Claude in Agentforce |
| 3 | **Token & Flex Credit Calculator** | Live sliders (reps + queries/day), real-time token math vs. Copilot RAG, latency comparison, Flex Credit cost |
| 4 | **Competitive Objection Matrix** | 3 flip-cards: Copilot cost objection, data safety objection, setup complexity objection |
| 5 | **CIO / SAM Pitch Track** | 4 value cards + comparison table vs. Microsoft Copilot |
| 6 | **Resources Footer** | 3 external link cards (Salesforce press release, Salesforce Ben, Trigger Hours) |

### Calculator Math (Verified to Rate Card)
- **Copilot RAG:** Reps × Queries × 30 days × 35,000 tokens/query
- **Claudeforce MCP:** Reps × Queries × 30 days × 1,500 tokens/query
- **Action Cost:** Reps × Queries × 30 days × 20 Flex Credits × $0.10/credit
- Token reduction: ~95.7% · Latency: 8.5s (Copilot) vs. 1.2s (Claudeforce)

---

## Site 2: External Public Explainer (`external.html`)

**Audience:** Customers, Prospects, General Public

**Design:** Light mode, clean and approachable
- White background, Salesforce Blue accent, professional but accessible tone

### Sections

| # | Section | Key Content |
|---|---|---|
| 1 | **Hero** | "The world's #1 CRM, now powered by Claude AI" — plain-English intro |
| 2 | **What Is Claudeforce** | Dark feature box with 4 key stats (37 skills, 0 integrations needed, 100% data in Trust Boundary, 7× faster) |
| 3 | **Why It Matters** | 3 value cards: CRM-native understanding, Zero Data Retention, no new complexity |
| 4 | **How It Works** | 3-step vertical flow: Salesforce in Claude → Claude in Agentforce → AIforce Layer |
| 5 | **Comparison** | Claudeforce vs. Generic AI feature table |
| 6 | **FAQ** | 5 accordion questions (what is it, data safety, setup time, product differences, availability) |
| 7 | **CTA Banner** | Link to official Salesforce announcement |

---

## File Structure

```
ClaudeForce - What is it/
├── index.html       # Internal AE Battlecard (dark mode, seller-only)
└── external.html    # External public explainer (light mode, customer-facing)
```

No build step. Pure HTML + Tailwind CDN + Lucide Icons + vanilla JS. Opens with `open index.html`.

---

## How to Update & Redeploy

```bash
cd "/Users/edalton/Desktop/Salesforce Cursor Projects/ClaudeForce - What is it"
# Edit files, then:
git add -A
git commit -m "your change description"
git push
# GitHub Pages auto-deploys in ~2 minutes
# Hard refresh: Cmd+Shift+R
```

---

## Key Messaging Reference

### Internal (AE Battlecard)
| Topic | Stat |
|---|---|
| Token savings vs. Copilot | ~95.7% |
| Copilot RAG tokens/query | 35,000 |
| Claudeforce MCP tokens/query | 1,500 |
| Copilot response latency | ~8.5s |
| Claudeforce response latency | ~1.2s |
| Prebuilt MCP sales skills | 37 |
| Flex Credit cost per action | $0.10 |
| Credits per action | 20 |
| Copilot active CRM task usage | ~8% |

### External (Customer Explainer)
- "The world's #1 CRM, now powered by Claude AI"
- Zero Data Retention — data stays inside Salesforce Trust Boundary
- 37 prebuilt sales skills, zero API setup
- Announced August 2026 — Salesforce + Anthropic partnership

---

*Built with Cursor AI · Hosted on GitHub Pages · Dreamforce 2026 Strategic Enablement*
*Questions: Eric Dalton — edalton@salesforce.com*
