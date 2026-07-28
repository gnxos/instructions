# LinkedIn Content Strategy — Instruction Brief (Gn Teja)

> **What this document is:** A standing reference brief for planning, generating, and evaluating LinkedIn content for this profile. Paste this in as context whenever drafting a post, brainstorming ideas, or searching for things to post about. It covers who to write for, what to write about, what currently performs on LinkedIn, and what to avoid.
>
> **Last updated:** July 2026 — repeatedly refined from an initial resume-driven draft: Section 5 opened from a fixed 4-pillar list into an expandable Core Domain + lanes model; Section 4's voice defaults shifted toward flat technical writing over founder narrative; opinion made optional rather than assumed on every post; and critique, when it does appear, aimed at patterns and tradeoffs rather than named people or companies. LinkedIn's algorithm and format preferences shift every few months too, so revisit Sections 6–8 periodically, keep Section 1 current as SuperOS.dev evolves, and add new lanes to Section 5 as material or opinions emerge.

---

## 1. Profile Owner — Key Facts

Use these as the source of truth for any credibility claims, numbers, or career details used in a post. Do not invent achievements or numbers not listed here.

- **Name:** Gnana Teja (goes by "Gn Teja" on LinkedIn) · 8+ years of experience
- **Location:** Austin, TX (Central Time)
- **Current status:** Technical Founder building SuperOS.dev; also open to the right full-time opportunity
- **GitHub:** Listed on the resume as a contact link — add the actual profile URL to LinkedIn's Featured section and Contact info
- **Career background** (most recent first):
  - **Founder, SuperOS.dev.** An AI low-code automation platform for ops teams to design and run no-code, agent-based workflows.
    - Built the core platform and workflow runtime in Go, with 100+ TypeScript-based tool integrations and Python/LangChain for AI orchestration
    - Designed three user-facing surfaces for the same agent capabilities: a spreadsheet-style layer, a drag-and-drop workflow builder, and a direct chat interface
    - Built core agent capabilities: skills, tool/function calling, RAG-based knowledge retrieval (document ingestion, embeddings, vector storage), guardrails, evals, and LangSmith tracing
    - Built a pluggable model layer supporting multimodal LLMs via OpenAI, Anthropic, and Gemini
    - Built a Model Context Protocol (MCP) bridge to connect enterprise data sources/tools into LLM workflows
    - Works directly with early users/design partners to scope use cases and iterate
    - Owns platform reliability end-to-end — orchestration behavior, integration versioning, retries/fallbacks, operational debugging — and mentors other developers
  - **Founder, AutoCRUD** (pivoted into SuperOS.dev). Built "Tables," a no-code spreadsheet-based platform letting non-technical users create/query live databases without SQL — now powers SuperOS.dev's production data layer. Built a database abstraction layer spanning relational, key-value, and analytical engines (PostgreSQL, MySQL, Redis, MotherDuck) behind one unified API.
  - **Senior Software Engineer, Tesla.** Engineering lead for WarpCDC, a Debezium + Kafka change-data-capture platform for Tesla's Warp data pipelines, at ~1.6B events/day, with end-to-end ownership of architecture, scaling, infra provisioning, connectors, and reliability. Owned evaluation and onboarding of Dgraph (working directly with the vendor) as a v2 data layer for entity relationships, search, and data exploration inside Workbench. Led development across Workbench and BPM (Tesla's case-management/automation systems) at millions of requests/day. Led onboarding of Cycles (Tesla's asset management/IT support system) into Workbench, including the migration off ServiceNow. Contributed to InstallBase (Tesla's system of record for Superchargers) and led automation for publishing Supercharger info across Google Maps, GMB, Instagram, and X — partnering directly with Google's Maps team.
  - **Software Engineer, Google.** Worked on Skyvine (Google's internal case-management platform), including V4 API features like email threading, notifications, and survey implementation. Forward-deployed across 20+ teams — including YouTube, Waymo, and Google Cloud — later staffed exclusively on Google Cloud Sales to support their migration from Salesforce to Skyvine. Built production services on Spanner and Pub/Sub using Java, Protobufs, gRPC, and TypeScript. Built dashboards/reporting with Stackdriver, PLX, and Data Studio.
  - **Full Stack Engineer, Reliable Software Resources.** Built backend services (Java/Spring Boot) and Terraform automation for a self-serve infrastructure-provisioning SaaS for data engineering/ML teams, deployed on AWS and PCF.
- **Education:** M.S. Computer Science, Texas A&M University-Kingsville · B.Tech Electronics & Communication, JNTU Anantapur, India
- **Certifications:** AWS Certified Developer Associate · PCF (Pivotal Cloud Foundry) Certified Developer · Google Associate Cloud Engineer
- **Network:** Hustle Fund Angel Squad member — a paid community of 1,500+ angel investors with access to Hustle Fund's vetted deal flow. A real, engaged network, not just a resume line.
- **Stated focus area:** AI infrastructure, agentic workflows, platform engineering, LLM productization
- **Broader technical expertise:** Go, Java, Python, JavaScript/TypeScript · distributed systems · GenAI/LLM apps (RAG, tool calling, evals, guardrails, multi-model orchestration) · Model Context Protocol (MCP) · microservices · API design (REST, GraphQL, gRPC) · Kafka & event streaming · databases (Dgraph, DynamoDB, PostgreSQL, MySQL, SQL Server, Redis, MotherDuck) · CI/CD, Docker, Kubernetes · AWS (Lambda, EC2, S3, SQS/SNS, IAM) · GCP (Compute Engine, Spanner, Pub/Sub, Data Studio)

## 2. Goals

1. **Prove AI/engineering proficiency** — technical credibility in distributed systems, AI infrastructure, and GenAI/agent engineering.
2. **Build visibility for SuperOS.dev** — attract high-quality connections (founders, operators, investors) and early customers/design partners, so there's already an engaged audience around what's being built.
3. **Surface the right next opportunity** — should happen as a byproduct of #1 and #2, not through separate "job search" content.

## 3. Target Audience

| Priority | Audience | Why they matter | What earns their attention |
|---|---|---|---|
| 1 | AI/infra engineers & technical leaders (staff/principal engineers, eng managers at AI-native or platform teams) | Credibility audience — their engagement is proof of expertise | Specific technical detail, real numbers, real tradeoffs |
| 2 | Founders, operators, early-stage investors (incl. Hustle Fund/Angel Squad network) | Future collaborators, hires, investors, and an audience for SuperOS.dev | Sound judgment, an investor/operator lens, genuine substance |
| 3 | Ops/RevOps/BizOps/IT leaders (potential SuperOS.dev users) | Real customers and design partners for the product | Concrete before/after workflow stories, real automation outcomes |
| 4 | Recruiters & hiring managers | Surfaces the next role | A keyword-searchable profile and credibility signals from #1–#3 |

## 4. Voice & Tone

- Specific over generic — real numbers, real systems, real decisions. Never vague claims.
- Direct, plain language. No corporate buzzwords ("passionate," "innovative thought leader," "disruptor," "guru," "synergy," etc.)
- Confident, not salesy — an engineer/founder's voice, not a marketer's
- Default opening is the technical claim, problem, or system behavior — not "I." Lead with the argument; save the personal frame for when it's genuinely the point.
- First person still shows up constantly, but as support for an argument, not as narration — stating a judgment ("I'd pick X over Y here"), owning a call, or citing something seen firsthand. Personal experience (SuperOS.dev, Tesla, Google) is evidence pulled in when it's the sharpest available proof — not the shape the post is built around.
- Opinion or critique isn't mandatory on every post. Plenty of good posts are just a genuine, specific reaction — an interesting fact, real curiosity about how something plays out — with no forced technical take attached. Don't manufacture an angle where the news doesn't need one.
- Critique the pattern, not the people, on the posts where there is a real opinion. Don't imply that a specific named person or company missed, overlooked, or got something wrong unless it's something you can actually back up. A genuine point about a tradeoff or a hard problem stands on its own without needing to cast someone else's work as lacking.
- Admitting what you'd do differently reads as credible, not weak — use it
- Stay on one thread per post — don't drag in unrelated personal context (a Tesla aside in a post about SuperOS.dev, or vice versa) unless it's directly necessary to make the point. One post, one topic.

## 5. Core Domain & Content Lanes

**Core domain:** how AI/agent systems — and the companies building them — get designed, built, operated, and evaluated. Technical architecture, product decisions, infra tradeoffs, and the investor/operator view of that same world. LinkedIn's ranking system rewards accounts that stick to a consistent domain — that consistency is what lets it learn the account's expertise and distribute content beyond the existing network.

The domain is the constraint, not the lane list below. Lanes are starting points, not a closed set — the moment something earns a new one (a framework, a paper, an industry shift, a sharp opinion that doesn't fit an existing lane), it gets added rather than shelved for not fitting one of a fixed four. Use the fit-check in Section 12 to decide fast.

Default mode is flat and factual — the claim, the system, or a genuine reaction, not the founder journey. Opinion is welcome when there's a real one behind it; it isn't a requirement for every post. Personal narrative is one lane among several, not the frame everything else sits inside.

**Lane — AI Infrastructure & LLM Productization POV (default lane — post here most often)**
Reactions to and analysis of the space, informed by building SuperOS.dev day to day but not narrated as a founder story. Not every post here needs a strong opinion — a specific, genuine observation or real curiosity about how something plays out counts too. This is what reaches people outside the existing network and does the most direct work for Goal #1 (technical credibility).
- Takes on agentic workflow design, RAG architecture, evals/guardrails approaches, multi-model orchestration, inference cost
- What's overhyped vs. genuinely useful in current agent/LLM tooling
- A builder's technical reaction to notable AI infra launches (MCP ecosystem moves, new models, agent frameworks)

**Lane — Systems Engineering: General Technical Writing**
Not narrated as "at Tesla, we..." every time — credibility through depth, not résumé.
- CDC/event-streaming patterns, schema evolution, backpressure handling
- Graph vs. relational vs. document databases — real tradeoffs, when to use what
- Workflow/orchestration system design, on-call and reliability practices
- Cloud architecture tradeoffs across AWS, GCP, and Pivotal

**Lane — Building SuperOS.dev (Engineering Decisions & Product)**
Real, current material, written as engineering decisions with tradeoffs — not chapters in a founder journey.
- The AutoCRUD → SuperOS.dev pivot as an architecture/product case study: why "Tables" (the no-code spreadsheet database) became the data layer, and what the shift toward agent-based workflow automation actually required
- Building a Model Context Protocol (MCP) bridge to connect enterprise data/tools into LLM workflows — what it unlocks, what's hard about it
- Why a pluggable multi-model layer (OpenAI, Anthropic, Gemini) instead of betting on one provider
- Designing three interfaces — spreadsheet layer, drag-and-drop builder, chat — for the same underlying agents, and what changed based on who's using it
- What "production-ready and reliable" actually takes for agents: guardrails, evals, LangSmith tracing, retries/fallbacks
- Lessons from working directly with early design partners to scope and refine automation use cases
- Zero-to-one lessons: codifying LLM orchestration best practices while mentoring other developers

**Lane — Scaling & Systems Proof: Tesla, Google & Beyond**
Deep infra credibility that pre-dates the startup — direct, named experience.
- Leading WarpCDC (Debezium + Kafka CDC) to ~1.6B events/day, and everything that came with owning it end-to-end
- Evaluating and onboarding Dgraph as a graph database — working directly with the vendor — and what changed once entity relationships had a proper v2 data layer
- Migrating Tesla's IT/asset-management system off ServiceNow (the Cycles → Workbench integration)
- Automating how Supercharger info stays accurate across Google Maps, GMB, Instagram, and X — partnering directly with Google's Maps team
- Forward-deployed engineering across YouTube, Waymo, and Google Cloud Sales — and what changed moving from Google's Skyvine platform to Tesla's BPM/Workbench systems

**Lane — The Investor/Operator Lens (occasional — not on rotation)**
A rare combination — deep infra experience, an active startup, and an angel-investing seat. Use when there's a genuine pattern worth sharing, not on a schedule.
- What to look for as an engineer turned angel investor — now with a founder's-eye view too, since you're building (and likely fundraising) yourself
- Lessons from evaluating deal flow through Hustle Fund/Angel Squad
- What makes a technical founder fundable, from an operator's perspective

**Next lane — open**
Whatever clears the fit-check in Section 12 and doesn't belong in any lane above gets its own new lane here, rather than getting forced into one of the above or dropped for not matching.

## 6. What Performs Right Now / What Doesn't (as of 2026)

**Performs well:**
- Document/carousel posts, 8–12 slides — currently the highest-engagement format. Keep slide count tight; low completion rates hurt distribution.
- Native video, uploaded directly (never linked from YouTube)
- Text posts with a strong hook in the first 2–3 lines, backed by specific numbers or a real story
- A genuine question at the end, when it fits naturally

**Actively suppressed — avoid:**
- Polls — engagement has collapsed to near-zero
- "Agree? Comment below 👇" style engagement bait
- Outbound links in the post body (~60% reach penalty; a link in the first comment no longer avoids this)
- Automated posting/commenting tools, engagement pods, or generic AI-written text

## 7. Posting Playbook

**Do:**
- Open with a hook that works in the first 2–3 lines — that's all most readers see before "see more"
- Default to leading with the technical claim, problem, or system behavior — not a personal opener. Bring in the personal frame only when it's genuinely the point.
- Use specific numbers, systems, and decisions instead of generic advice
- Reply to every comment fast, especially within the first hour
- Spend real time commenting thoughtfully on other people's posts — Angel Squad members, Hustle Fund GPs, respected AI infra engineers, and people building in the MCP/agent-tooling space. Often a faster lever than original posting.
- Stay within the Core Domain in Section 5 — the lanes underneath it can and should expand

**Don't:**
- Post outside the Core Domain — "unrelated" is judged against the domain statement in Section 5, not against a fixed topic list, so a new lane within the domain is always fair game
- Pad a single post with tangential personal backstory pulled from a different lane (e.g., a Tesla story dropped into a SuperOS.dev post) — stay on the one thing that post is actually about, unless the extra context is genuinely necessary to make the point
- Post vague, low-substance "building in public" filler — there's enough real material now to always be specific
- Rely on outbound links, polls, or engagement bait
- Use automation for posting or commenting

## 8. Cadence & Timing

- **Frequency:** 2–3 posts/week minimum, up to 5/week if quality holds. Fewer substantive posts beat frequent filler.
- **Best days/times:** Tuesday–Thursday, 10am–12pm Central Time (Austin). Wednesday is typically the strongest single day. This window overlaps with mid-to-late morning Pacific Time, useful for reaching the VC/founder audience.
- **First hour after posting matters most** — the critical window for replying to comments and driving the early engagement that determines wider distribution.

## 9. Profile Reference

**Headline — pick one:**
1. Founder, SuperOS.dev — AI Agent Workflow Automation | Ex-Tesla, Ex-Google | Kafka CDC @ 1.6B events/day
2. Building SuperOS.dev (AI agents for ops teams) | 8+ yrs Distributed Systems & GenAI | Ex-Tesla, Ex-Google
3. Technical Founder @ SuperOS.dev | Agentic Workflows, RAG, MCP | Ex-Tesla, Ex-Google

**About section draft:**

I'm building SuperOS.dev — a no-code platform that lets operations teams design and run production-ready, agent-based workflows without needing an engineering team to maintain them.

Before this, I spent 8+ years owning distributed systems end-to-end: leading WarpCDC, a Kafka-based change-data-capture platform running ~1.6B events/day at Tesla; onboarding Dgraph as a new v2 data layer; and working forward-deployed across 20+ teams at Google, including YouTube, Waymo, and Google Cloud Sales.

SuperOS.dev started as AutoCRUD, a no-code database platform — we pivoted after seeing what teams actually needed was agent-based automation, not just data tooling. Today the platform runs on a pluggable multi-model layer (OpenAI, Anthropic, Gemini), with RAG, guardrails, evals, and a Model Context Protocol bridge into enterprise systems.

I'm also part of Hustle Fund's Angel Squad, investing in and learning from early-stage founders.

Always up for a conversation with engineers, founders, operators, or investors working on AI agents, infra, or workflow automation — and open to the right next opportunity if it's a strong fit.

**Featured section:** Add the GitHub profile, and a SuperOS.dev link if there's a public landing page — tangible proof outperforms claims.

## 10. Existing Network to Leverage

- Hustle Fund Angel Squad: 1,500+ member community of angel investors/operators — a built-in warm audience
- Early users/design partners of SuperOS.dev — worth featuring (with permission) as proof points
- Priority engagement targets: Angel Squad members, Hustle Fund GPs, AI infra engineers, and people building in the MCP/agent-tooling ecosystem

## 11. What to Expect

- Meaningful engagement typically doesn't show up until roughly week 4–6 of consistent, quality posting — normal, not a sign the strategy isn't working
- Platform-wide organic reach is down significantly year-over-year for everyone as of 2026 — slow early traction is the current baseline
- Fewer than 2% of LinkedIn members post weekly — consistency alone is a differentiator

## 12. Quick-Use Instructions (for drafting a specific post)

When generating a LinkedIn post idea or draft from this brief:
1. Run the fit-check (~10 seconds, two questions):
   - **Domain check** — does this touch how AI/agent systems, or the companies building them, get designed, built, run, evaluated, or invested in?
   - **Substance check** — is there a real number, decision, tradeoff, or opinion here, not just commentary?
   Both yes → write it, in whichever lane from Section 5 fits best. No need for a perfect match — if nothing existing fits, that's a new lane, not a reason to cut the idea.
2. Default to the flat technical explainer/opinion shape — no personal anecdote required. Pull a specific number, decision, or story from Section 1 only when personal experience is genuinely the sharpest available evidence for the point — never to manufacture relatability, and never invented.
3. Keep the post anchored to that single lane/topic. Don't drag in unrelated personal context from a different lane (a Tesla story in a SuperOS.dev post, or vice versa) unless it's genuinely necessary to the point — cut it if it's just there to sound more personal or credible.
4. Draft a 2–3 line hook that works standalone — leading with the claim or system, not "I."
5. Match the voice in Section 4.
6. Recommend carousel format for technical/step-based content, native video for a quick take, plain text for opinions/stories.
7. End with a genuine question or a light, non-pushy CTA — never a hard sales pitch.
8. No outbound links in the post body, no polls, no engagement-bait phrasing.
9. Check the draft against Sections 6–7 before finalizing.

---

*Reflects LinkedIn platform/algorithm research as of July 2026, updated with founder/product details from the July 2026 resume. Revisit periodically — format performance and algorithm behavior shift, and Section 1 should be kept current as SuperOS.dev evolves.*
