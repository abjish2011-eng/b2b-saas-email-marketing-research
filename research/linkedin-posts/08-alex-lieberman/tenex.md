# Tenex

- Author: Alex Lieberman
- LinkedIn Post Caption: copied from CSV
- Date Collected: 2026-07-08
- Source Type: Copy-pasted LinkedIn post from CSV

## Post Text

People made fun of Alex Finn for buying three Mac Studios to run AI at home.

Then Fable got banned for a week, GLM 5.2 dropped, and those exact Mac Studios started reselling for 4x what he paid.

He showed me how he built his home AI lab from scratch. Here's the playbook:

1) The hardware. three 512GB Mac Studios, an NVIDIA DGX Spark, a custom RTX 5090 build, and a few Mac Minis. ~$30k all in.

2) The buying framework... 
- Mac Studio: huge memory, runs GLM 5.2 (open weights, near Opus 4.8 on benchmarks), but slow. 
- DGX Spark ($4,800): the sweet spot for most people. 
- RTX 5090: smaller models at blazing speed (Qwen's 29B now hits Sonnet 4 level). 

3) Tailscale networks every machine into one private network with root access to each other. Only one machine is plugged into a monitor.

4) A Nous Research Hermes agent is his IT guy. New model drops? It SSHs into the right box, loads 5 candidates, runs evals overnight, and reports back which task belongs on which machine. Alex has literally never loaded a model himself.

5) The whole point: achieving "ambient intelligence." Always-on jobs that would bankrupt you on per-token billing. A security sweep of his API endpoints every hour. Code optimization every 20 minutes. Database anomaly & churn detection. Hourly scraping of X, Reddit & Hacker News for business opportunities.

6) Running those workloads on frontier models would cost thousands a month. His actual cost: ~$60 more in electricity.

7) Btw he's not anti-frontier. He still maxes out his Claude plan. The way he sees it: frontier is for hard thinking, local is for the foot soldiers that never sleep.

8) "We own everything except for the intelligence. Why can't we own the intelligence?"

9) He thinks frontier-level intelligence runs on consumer hardware within 6 months.
