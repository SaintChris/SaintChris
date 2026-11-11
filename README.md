![SAINTLEX. Alex Bogle, AI Engineering and Automation. IoT and AI Technician at IREE Solar, Jamaica.](assets/banner.png)

# Alex Bogle | AI Engineering & Automation

I build practical AI systems, agents, workflows and integrations, and I ship them tested, secured and documented.

**Current role:** IoT & AI Technician at IREE Solar, Jamaica. AI Engineering & Automation is the discipline, not the job title.

## Work at IREE Solar

Each item has its status and, where I have one, a measured result. Full write-ups are on [saintlex.sbs](https://saintlex.sbs/#work).

- **Staff assistant.** Answers staff product questions from 118 manufacturer documents and names the source. Grok 4.7 with hybrid search (BM25 and bge-base) and a MiniLM reranker, plus prompt and output guards. On a 62-question test set it gets 62 right, against 25 for plain Grok, which made up figures in 18 answers. *Staff pilot.* [Case study](https://saintlex.sbs/case-studies/staff-assistant/)
- **Website chat.** Answers only from approved company facts and hands anything else to a person. 37 of 37 test answers right by hand, 11 of 11 red-team attacks refused. *Waits for the new site.* [Case study](https://saintlex.sbs/case-studies/website-chat/)
- **Server, backups and monitoring.** A Linux server behind Cloudflare, with an encrypted nightly backup on a separate machine. The monthly restore drill brings back 6.1 GB in 92 seconds, and 99.67% of 221,364 uptime checks passed over 29 days. Two written postmortems. *In use.* [Case study](https://saintlex.sbs/case-studies/server-backups-and-recovery/)
- **Guard rails for AI coding agents.** Three guards check every shell command an agent runs: keys only go to their own service, no pushes to main or force-pushes, and no endless sleep blocks. 24 agent skills written from vendor documentation. *In use.*
- **Monitoring alerts and customer reports.** A daily watch of equipment alerts, matched to each customer's service history, and plain-language performance reports for 15 battery sites so far. *In use.*
- **Field service.** Water heater repairs, inverter alert call-outs, site surveys, and Powerwall warranty follow-up with Tesla. *Since September 2026.*
- **Field automation.** Website, ServiceM8 and Zoho workflows where a person approves every live write. Built and tested, then paused on 7 November 2026; two small read-only tools are live. *Paused.*
- **GitHub.** 726 merged pull requests since August 2026, most written with coding agents and reviewed by me. 43 workflows across 19 repositories. When the included Actions minutes ran out on 20 October 2026, I moved CI to 7 self-hosted runners on company machines: about 1,340 minutes a month projected, against about 9,000 if every job ran on GitHub.

These repositories are private.

## Featured work

| Repository | What it is | Category |
| --- | --- | --- |
| [agentic-systems-lab](https://github.com/SaintChris/agentic-systems-lab) | Six agent roles on a shared task queue, a dashboard that runs on demo data, tests in CI | Lab |
| [iot-energy-telemetry-lab](https://github.com/SaintChris/iot-energy-telemetry-lab) | Synthetic solar and battery telemetry over MQTT: device identity, topic design, JSON validation, offline tests | Lab |
| [sp-agent-session-sync](https://github.com/SaintChris/sp-agent-session-sync) | Puts Claude Code, T3 Code, Codex and Grok sessions onto the matching Super Productivity task | Personal project |
| [omarchy-super-productivity](https://github.com/SaintChris/omarchy-super-productivity) | Omarchy bar widget for the current task and today's time, with start and stop | Personal project |
| [saintlex.sbs](https://saintlex.sbs/) | My portfolio site: work, case studies with measured results, and open source (private repository) | Personal project |

The RAG evaluation lab is private for now.

## Open-source contributions

Shipped:

- [Open WebUI iOS app](https://github.com/JoaoZaokk/openwebui-ios/issues/15): my feature write-up became follow-up suggestion buttons under each answer. Credited as co-author on [ff1ae6e](https://github.com/JoaoZaokk/openwebui-ios/commit/ff1ae6e).
- [Super Productivity](https://github.com/super-productivity/super-productivity/pulls?q=is%3Apr+author%3ASaintChris+is%3Amerged): local REST API routes to log time on a given day ([#10826](https://github.com/super-productivity/super-productivity/pull/10826)) and for notes ([#10827](https://github.com/super-productivity/super-productivity/pull/10827)), and a flag to start the app minimized ([#11321](https://github.com/super-productivity/super-productivity/pull/11321)).
- [awesome-second-brain](https://github.com/aristoapp/awesome-second-brain/pull/19): setup guide, example workflow, comparison pages and solution profiles.
- [ed-donner/agents](https://github.com/ed-donner/agents/pull/1414): week 1 notes in the community contributions of the agentic AI course.

In review:

- Super Productivity: tag and project write routes ([#10828](https://github.com/super-productivity/super-productivity/pull/10828)), a port flag so two profiles can each run the REST API ([#11432](https://github.com/super-productivity/super-productivity/pull/11432)), and custom titles for calendar time blocks ([#11438](https://github.com/super-productivity/super-productivity/pull/11438)).
- [Chroma](https://github.com/chroma-core/chroma/pull/7230): Haystack integration examples for the docs.
- [HermesHub](https://github.com/amanning3390/hermeshub/pull/119): open-source contribution and platform-picker skills.

## Engineering principles

- Read before changing. Find out what the system does now and what must still work afterward.
- Collect evidence: logs, data and the actual error.
- Make small changes I can undo, with a restore point first.
- Keep secrets and customer data out of code, notes and public pages.
- Verify against the test, then write down what changed.
- I use AI coding agents for much of the implementation. I set the scope, review the output and check the result myself before it ships.

## Stack

- **Daily:** Linux, Bash, Git, Docker, GitHub Actions with self-hosted runners, Python, Node.js, TypeScript, Rust.
- **AI and data:** Grok, Open WebUI, hybrid search (BM25 and embeddings) with a reranker, evaluation sets with baselines, prompt and output guards, AI coding agents (Claude Code, Codex, Grok).
- **Automation and integration:** n8n, REST APIs, ServiceM8, Zoho, Google Workspace, Cloudflare.
- **Operations:** restic backups with restore drills, Uptime Kuma, Healthchecks.io, ntfy alerts, Trivy image scans.
- **Energy systems:** Tesla Powerhub and Powerwall, Fronius, eGauge, WeCo, solar and battery monitoring, outage and reserve analysis.
- **Foundation:** device and firmware troubleshooting, networking diagnostics.
- **Learning:** AWS fundamentals, MQTT and IoT integration (lab only).

## Links

- Portfolio: [saintlex.sbs](https://saintlex.sbs/)
- LinkedIn: [alex-bogle](https://www.linkedin.com/in/alex-bogle/)
- Email: [bogle.alex@hotmail.com](mailto:bogle.alex@hotmail.com)

Forks on this account are reference material, not my own work.
