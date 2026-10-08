# Hacktober 2026: 14 Hackathons, Ranked by Odds of Winning

*Prepared Oct 4, 2026. Ranking is my judgment, not data. It weighs: how many winning slots exist, how niche the challenge is (fewer strong entrants), and how well it fits time-series / quant modeling, LLM orchestration, agents and cloud work. "Odds" are tiers, not percentages.*

**Read this first**
- Dates and prizes come from the list you shared plus a few searches. Only a handful were independently confirmed. **Open each official page and check rules, eligibility (country, age, student status) and the real deadline before you commit.**
- ETH Lagos 2026 could not be verified from any source other than the list.
- The Nigeria slots are thin. Only ETH Lagos and (loosely) MDBA / BLI are Lagos-linked; the rest are online and open to Nigerians. Decide if that counts as your "7 Nigeria".
- Trading-agent hackathons (Bitget, WEEX, Binance) sometimes geo-restrict or require KYC for prizes. Check this before building.

---

## The Ranked List

| # | Event | Track | Deadline / Dates | Prize | Odds | Best possible outcome |
|---|-------|-------|------------------|-------|------|-----------------------|
| 1 | **[Nebius x NVIDIA Global AI Hackathon](https://nebiusglobalaihackathon.devpost.com)** | Global | Closes Oct 30 | $50K+ total, 23+ slots | **Strong** | Top-3 cash + GPU credits, NVIDIA/Nebius visibility |
| 2 | **[OpenHackathons AI + HPC + Quantum](https://www.openhackathons.org/s/upcoming-events)** | Nigeria/EMEA (online/hybrid) | Oct 6-29 | Mentorship, compute access, certificates | **Strong** | Winning team recognition + HPC/GPU access and mentors |
| 3 | **[ForgeHacks Online 2026](https://forgehacks.dev)** | Nigeria (online, student) | Closes Oct 10 | Not listed | **Strong** | Category win + portfolio piece; low competition |
| 4 | **[BLI Legal Tech Hackathon 2](https://dorahacks.io/hackathon/legal-hack-2026)** | Nigeria (online) | Closes Oct 31 | $20K | **Decent+** | Prize + niche credibility in legal/regtech AI |
| 5 | **[Qloo Agentic Hackathon](https://qloo.devpost.com)** | Nigeria (online) | Closes Oct 30 | $25K cash | **Decent+** | Prize + a clean agent demo using a niche API |
| 6 | **[Open Agent Hackathon 2026](https://hackathon.genai.works)** | Global | Reg closes Oct 13, build Oct 15-20 | Up to $20K, 4 tracks + tinkerer track | **Decent** | Track prize; the tinkerer track gives a second shot |
| 7 | **[MDBA Youth Blockchain Hackathon](https://dev.events/hackathons/AF/NG/Lagos/tech)** | Nigeria (online) | Closes Oct 31 | Not listed | **Decent** | Youth-category win; low competition but needs blockchain work |
| 8 | **[Binance Agentic AI Challenge](https://dorahacks.io/hackathon/binance)** | Global | Closes Nov 13 | $6K | **Decent** | Prize reusing your trading-agent build |
| 9 | **[Bitget AI Hackathon S2](https://x.com/bitget_ai)** | Global | Oct 8 (verify start vs deadline) | $50K USDT | **Fair** | Top prize for an autonomous trading agent; quant fit is your edge |
| 10 | **[Google Gemma 4 Developer Agent Competition](https://www.kaggle.com/competitions/gemma-4-developer-agent)** | Global | Closes Nov 12 | $65K cash | **Fair** | Leaderboard placing; strong CV signal even without a win |
| 11 | **[WEEX AI Wars II](https://dorahacks.io/hackathon/weex-ai-wars2)** | Global | Closes Oct 12 | $200K | **Long shot** | Placing in a very large pool; huge upside, crowded field |
| 12 | **[ETH Lagos 2026](https://hacklist.io)** (unverified) | Nigeria (in-person, Lagos) | Oct 8-10 | Not listed | **Long shot** | Local win + networking with Lagos Web3 builders |
| 13 | **[Build, Ship, Shape: Amazon Developer Hackathon](https://amazonappdev2026.devpost.com)** | Global | Closes Oct 23 | $138K, 8+ cash prizes | **Long shot** | A cash prize + AWS credits; themes (Fire TV, Alexa+, Ring) are off your core |
| 14 | **[Qollab x IonQ Global Quantum Hackathon](https://qollab.xyz/programs/hackathon)** | Nigeria/online | **Reg closes Oct 6**, sprint Oct 9-11 | $10K cash + $20K compute | **Long shot** | Placing with a Qiskit entry; steep ramp-up, but your maths degree helps |

---

## Why these ranks

**Strong (1-3)**
- **Nebius x NVIDIA** has 23+ slots, so you only need to land in the top tier, not first place. It also matches agentic work on open-weight models.
- **OpenHackathons** is mentor-driven and regional, so there are fewer elite entrants than in global prize races.
- **ForgeHacks** is student-only and small. A polished AI project can plausibly take a category.

**Decent (4-8)**
- **BLI Legal Tech and Qloo** are niche. Few ML engineers will build for them, so a good LLM-orchestration demo stands out.
- **Open Agent Hackathon** has a tinkerer track, which improves your chance of placing somewhere.
- **MDBA** is a youth-only pool, but you would need a credible blockchain component.
- **Binance** has a smaller prize and likely a smaller field, and it reuses your trading-agent work.

**Fair to long shot (9-14)**
- **Bitget and WEEX** are big, public prize pools full of experienced quants and bot builders. Your forecasting and quant background is a real edge, but so many people will compete.
- **Gemma 4** is a Kaggle-style leaderboard competition. Strong teams and heavy compute are the norm.
- **Amazon** has big prizes but the themes are consumer-device focused.
- **ETH Lagos** is unverified, in-person, and needs smart-contract skills.
- **Qollab** closes in two days and needs quantum tooling.

---

## Shared-build plan (so 14 is realistic)

| Build | Used for |
|-------|----------|
| **Trading-agent stack** (time-series forecasting + LLM decision layer + risk rules) | Bitget, WEEX, Binance (#9, #11, #8) |
| **Agent with persistent memory + tool use** (AWS-hosted) | Open Agent, Qloo, Amazon, Nebius x NVIDIA (#6, #5, #13, #1) |
| **LLM contract/compliance analyzer** | BLI Legal Tech (#4), possibly MDBA |
| **Fine-tuning pipeline for open models** | Gemma 4, Nebius x NVIDIA (#10, #1) |
| **Small standalone projects** | ForgeHacks, OpenHackathons, ETH Lagos, Qollab (#3, #2, #12, #14) |

Three core builds cover most of the list. That is what makes 14 entries possible.

---

## Deadline order (what to do first)

1. **Oct 6**: Qollab x IonQ registration closes. Decide today whether to enter or drop it.
2. **Oct 8**: Bitget S2; ETH Lagos starts (Oct 8-10).
3. **Oct 10**: ForgeHacks closes.
4. **Oct 12**: WEEX AI Wars II closes.
5. **Oct 13**: Open Agent registration closes (build Oct 15-20).
6. **Oct 23**: Amazon Developer Hackathon closes.
7. **Oct 29**: OpenHackathons window ends (starts Oct 6).
8. **Oct 30**: Nebius x NVIDIA and Qloo close.
9. **Oct 31**: BLI Legal Tech and MDBA close.
10. **Nov 12-13**: Gemma 4 and Binance close.

## If you need to cut

Drop in this order: **Qollab, Amazon, ETH Lagos, WEEX.** That still leaves 10 entries with the strongest odds and best skill fit, and you can swap in Nigeria-based events if they turn up.

## Not counted

Hacktoberfest (open-source contributions, not a hackathon), and closed Nigerian events: HelpMum CareCode 2.0 (July), Web3Lagos Conference (August), NASENI FutureMakers (August, ages 5-16). GTCO Squad 3.0 is student-only; check [squadco.com/hackathon](https://squadco.com/hackathon) for current timing and add it if it is open.

---

## Links

*These URLs come from the list you shared plus my searches. I opened only a few of them, so confirm each page loads and shows the right event. The MDBA and ETH Lagos links are aggregator pages, not official event pages.*

| # | Event | Link |
|---|-------|------|
| 1 | Nebius x NVIDIA Global AI Hackathon | <https://nebiusglobalaihackathon.devpost.com> |
| 2 | OpenHackathons AI + HPC + Quantum | <https://www.openhackathons.org/s/upcoming-events> |
| 3 | ForgeHacks Online 2026 | <https://forgehacks.dev> |
| 4 | BLI Legal Tech Hackathon 2 | <https://dorahacks.io/hackathon/legal-hack-2026> |
| 5 | Qloo Agentic Hackathon | <https://qloo.devpost.com> |
| 6 | Open Agent Hackathon 2026 | <https://hackathon.genai.works> |
| 7 | MDBA Youth Blockchain Hackathon | <https://dev.events/hackathons/AF/NG/Lagos/tech> |
| 8 | Binance Agentic AI Challenge | <https://dorahacks.io/hackathon/binance> |
| 9 | Bitget AI Hackathon S2 | <https://x.com/bitget_ai> |
| 10 | Google Gemma 4 Developer Agent Competition | <https://www.kaggle.com/competitions/gemma-4-developer-agent> |
| 11 | WEEX AI Wars II | <https://dorahacks.io/hackathon/weex-ai-wars2> |
| 12 | ETH Lagos 2026 | <https://hacklist.io> |
| 13 | Build, Ship, Shape: Amazon Developer Hackathon | <https://amazonappdev2026.devpost.com> |
| 14 | Qollab x IonQ Global Quantum Hackathon | <https://qollab.xyz/programs/hackathon> |

**Discovery hubs for more events**
- DoraHacks: <https://dorahacks.io/hackathon>
- dev.events (Lagos tech hackathons): <https://dev.events/hackathons/AF/NG/Lagos/tech>
- dev.events (Lagos AI hackathons): <https://dev.events/hackathons/AF/NG/Lagos/ai>
- GTCO Squad Hackathon: <https://squadco.com/hackathon>
