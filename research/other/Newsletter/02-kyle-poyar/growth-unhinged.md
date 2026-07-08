# What AI-native GTM looks like at public company scale

- Author: Kyle Poyar
- Newsletter Link: https://www.growthunhinged.com/p/what-ai-native-gtm-looks-like-at-public-company-scale
- Date Collected: 2026-07-09
- Source Type: Public newsletter issue page

## Newsletter Text

Growth Unhinged is proudly supported by beehiiv

Growth Unhinged is, quite literally, powered by beehiiv. I made the switch at the beginning of the year because beehiiv is serious about powering the internet’s best newsletters. Their all-in-one platform brings together newsletters, websites, and every tool you need to grow and earn.

It’s now even better with the new beehiiv MCP. I use the MCP in Claude Cowork to audit my site and prioritize SEO fixes, analyze subscriber trends, and set up automations. And they aren’t stopping — see what beehiiv is cooking up at their big Summer Release 26 on July 16th. See beehiiv yourself and get 30% off for three months with code KYLE30.

See the beehiiv difference
In 2026 alone, monday.com's AI agents handled tens of thousands of leads, booked thousands of meetings, and generated millions of dollars in pipeline. Demo request response times dropped from 24 hours to under 2 minutes. This is real AI GTM in production at a $1B+ ARR company.

I've been following AI GTM closely — I wrote a 60-page report on it earlier this year — but what doesn't get talked about is what happens when these plays collide with intricate routing logic, global rollouts, legacy tech stacks, and real compliance requirements.

Then I got connected to Oran Akron, the VP of AI for GTM at monday. Oran built monday’s RevOps org from zero to 80+ people over nearly 8 years. Last year he was tasked with creating an internal startup to rethink GTM workflows using AI agents (they call it RevAI). The scale here is wild: a publicly traded company growing 24% year-on-year with 1,000+ GTM employees.

I’ll show you three of monday’s most impactful AI GTM workflows, then unpack the messy work of building (and rebuilding) AI agents that work at enterprise scale.

Subscribe to Growth Unhinged
AI workflow 1: Inbound qualifying and hand-off agent
Internal name: Amanda

What it does: Qualifies inbound contact sales requests using voice agents and qualifies using BANT.

Results: The agent handles 100% of English-speaking “contact sales” inbound flows; AI agents respond within ~2 minutes (down from ~24 hours).

Oran needed a wedge case where AI agents could meaningfully improve the existing GTM approach. He quickly honed in on speed-to-lead; the faster the response, the higher the conversion to qualified meeting.

The AI GTM team built “Amanda” – an inbound qualifying and hand-off agent. Their philosophy: sales reps shouldn't handle leads; they should only receive qualified meetings with the context already prepared.

Amanda is set up as a dedicated user in monday's CRM that gets assigned leads as they come in. Lead assignment triggers orchestration across 20+ preparation workflows including insight gathering, timezone resolution, agent versioning, accent matching, and local phone number selection — all within 60 seconds of a 'contact sales' CTA submission.

From there, Amanda executes voice calls that last about 5 minutes on average. These are deployed in English-speaking markets along with places like Brazil, France, and Germany. I tested a call from Amanda and was pretty impressed by the experience. Some of the nuances of the call execution:

It clearly discloses this is AI and that calls are being recorded. The monday team brought some personality into it that I quite liked: “This call is being recorded so my creator knows I’m not causing chaos.” (LOL 😂)

The AI has a personality and some humor. The first line of the conversation is “You’ve been connected to a very enthusiastic robot.” This has been tested rigorously to minimize hang-up rates. (You can hear from Amanda by listening to the voice memo below.)

The conversations are objective-based. These aren’t scripted conversations (although the agent has guardrails for acceptable and unacceptable statements). Rather, they’re dynamic and the agent has specific objectives: (a) understand intent, ex: support vs. commercial interest, (b) identify their pain point, (c) assess needs, (d) verify buying authority, (e) clarify the use case, and (f) schedule the meeting with sales.

Latency issues can derail voice calls. The team targets 0.6-0.8 seconds between human speech and the AI agent’s response. They’ve needed to keep the knowledge base quite lean to minimize latency.

There are multiple sub-funnels after the call. These include human escalation, successful demo scheduling, and additional qualification paths. The AI agent has a ChiliPiper integration for meeting scheduling with automated calendar invites for both parties. A personalized voice memo gets created for the assigned rep and it’s shared via Slack. The AI updates monday’s CRM with all the relevant hand-off context.

Oran’s team was quite conservative in the initial deployment and A/B tested multiple iterations compared against manual outreach. Amanda has now organically spread across the org and well beyond the intended user base.

AI workflow 2: In-platform trial activation agent
Internal name: Jax

What it does: Pops up in the platform during free trial, identifies intent and potential, and routes users to the most optimal value.

Results: 2.5x conversion rate among Jax users compared to the control group.

monday has a PLG motion with a large volume of free trial signups. “Jax” — their trial activation agent — appears as an avatar in the bottom right corner of the app, acts as a personal sales engineer, available to talk live at any point during the free trial, and can take actions on the product frontend to configure custom instances.

They’ve seen promising early results with over 3,000 monthly calls, 50% of users coming back for a second call, and an overall increase in conversion to paid. Jax users convert at 2.5x the rate of the control group, according to Oran.

The team wasn't sure how users would respond. But they're seeing high engagement, and users miss Jax when the trial ends. That's not something you hear often about a sales automation tool.

AI workflow 3: Outbound research and account planning agent
Internal name: Oscar

What it does: Deep account research, account plans, and email cadences at scale.

Results: Tasks that previously took reps 1–2 weeks now take ~5 minutes. The monday team is still working on further visibility and ways to measure “time saved” and productivity increases (which will later be translated into ARR).

monday has an enterprise sales motion, too, and counts 60% of the Fortune 500 as customers. “Oscar” helps reps and territory managers go deeper on account strategy. Think: podcast listening, financial report analysis, internal platform usage data, combined into account plans with target departments, personas, and suggested outreach cadences.

Tasks that previously took reps 1–2 weeks now take ~5 minutes. Oscar is presented to reps as a single AI employee but is actually a set of orchestrated agents connected to Clay, LinkedIn (despite some frustrating API limitations), custom agentic solutions, and pre-AI enrichment tools the team had already licensed. It helps reps decide where the right opportunities are, how to stay current on those accounts, and how not to miss signals inside a company that can be turned into an opportunity.
