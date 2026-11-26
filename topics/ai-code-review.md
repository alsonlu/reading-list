# AI code review and automerge

Approaches and research on AI-assisted code review systems.

## Company and vendor write-ups

- [x] **[uReview](https://www.uber.com/us/en/blog/ureview/)** (Uber, 2025-08), found 2026-10-12 (from: bureau-code-review). Four-stage prompt chain with a grader on a different model; about 75% of rated comments useful, which showed how far thresholds and dedupe get you.
- [x] **[Building uReview (AI Engineer talk)](https://aiengineer.podhood.com/feb79ed8-7bf0-4a8d-8c2c-f00e78e435ed)** (Uber, 2026-08), found 2026-10-12 (from: bureau-code-review). 2026 update: routes each PR to a review depth and cut cost by 60% against the naive build.
- [x] **[How Uber uses AI for development](https://newsletter.pragmaticengineer.com/p/how-uber-uses-ai-for-development)** (The Pragmatic Engineer, 2026-03, paywalled), found 2026-10-12 (from: bureau-code-review). Context on Uber's AI developer tools, including the reviewer.
- [x] **[DoorDash built an AI code reviewer engineers actually listen to](https://careersatdoordash.com/blog/doordash-built-an-ai-code-reviewer-engineers-actually-listen-to/)** (DoorDash, 2026-05), found 2026-10-12 (from: bureau-code-review). Lead scout plus deep reviewers with a disprove-it pass; reports the share of high-severity findings that changed code.
- [x] **[How the Claude Code team does code review](https://claude.dev/blog/solving-code-review-at-anthropic/)** (Anthropic, 2026-10-15), found 2026-10-12 (from: bureau-code-review). Verify-and-vote on findings, risk tiers and convergence rules; used as the yardstick when comparing review setups.
- [x] **[Code Review](https://claude.com/resources/articles/code-review)** (Anthropic, 2026), found 2026-10-12 (from: bureau-code-review). Managed reviewer whose agent team scales with PR size; notable for the very low share of findings marked incorrect.
- [x] **[Code Review docs](https://code.claude.com/docs/en/code-review)** (Anthropic, 2026), found 2026-10-12 (from: bureau-code-review). Setup and behaviour of the managed PR reviewer.
- [x] **[claude-code repository](https://github.com/anthropics/claude-code)** (Anthropic), found 2026-10-12 (from: bureau-code-review). Its code-review plugin shows a compliance-plus-bug agent layout with one validator per issue.
- [x] **[60 million Copilot code reviews and counting](https://github.blog/ai-and-ml/github-copilot/60-million-copilot-code-reviews-and-counting/)** (GitHub, 2026-03), found 2026-10-12 (from: bureau-code-review). Moving to an agentic reviewer with repo context raised positive feedback, and it stays silent on many reviews.
- [x] **[ReviewBench: an open benchmark for AI code review](https://github.blog/ai-and-ml/github-copilot/reviewbench-an-open-benchmark-for-ai-code-review/)** (GitHub, 2026-10), found 2026-10-12 (from: bureau-code-review). Open benchmark; a multi-model ensemble improved precision and recall at lower cost.
- [x] **[ReviewBench leaderboard](https://review-bench.ai/)** (GitHub, 2026-10), found 2026-10-12 (from: bureau-code-review). F1 scores for AI reviewers, useful as a rough comparison point.
- [x] **[A Practical Approach to Verifying Code at Scale](https://alignment.openai.com/scaling-code-verification/)** (OpenAI, 2025-12), found 2026-10-12 (from: bureau-code-review). Reviewer trained for precision that runs code; argues verifying a finding is far cheaper than generating it.
- [x] **[Building a better Bugbot](https://cursor.com/blog/building-bugbot)** (Cursor, 2026-01), found 2026-10-12 (from: bureau-code-review). Biggest gains came from one agent deciding where to dig instead of many voting passes.
- [x] **[Bugbot now self-improves with learned rules](https://cursor.com/blog/bugbot-learning)** (Cursor, 2026-04), found 2026-10-12 (from: bureau-code-review). Learns rules from reviewer feedback to suppress low-value comments.
- [x] **[Bugbot is now over 3x faster](https://cursor.com/blog/bugbot-updates-june-2026)** (Cursor, 2026-06), found 2026-10-12 (from: bureau-code-review). Latency update with resolution-rate numbers.
- [x] **[How to Make LLMs Shut Up](https://www.greptile.com/blog/make-llms-shut-up)** (Greptile, 2024-12), found 2026-10-12 (from: bureau-code-review). Filtering comments that resemble downvoted ones lifted the addressed rate sharply.
- [x] **[Greptile v4](https://www.greptile.com/blog/greptile-v4)** (Greptile, 2026-03), found 2026-10-12 (from: bureau-code-review). Earlier architecture, the baseline for v5.
- [x] **[Greptile v5](https://www.greptile.com/blog/greptile-v5)** (Greptile, 2026-08), found 2026-10-12 (from: bureau-code-review). Swarm with one agent per hypothesis raised the addressed rate and halved latency.
- [x] **[How to build a code review agent](https://www.greptile.com/blog/how-to-build-a-code-review-agent)** (Greptile, 2026-10), found 2026-10-12 (from: bureau-code-review). Practical design guide; some claims are unmeasured.
- [x] **[CodeRabbit architecture](https://docs.coderabbit.ai/overview/architecture)** (CodeRabbit, 2026), found 2026-10-12 (from: bureau-code-review). Review and verification agents plus many analyzers; marketing-level, no published method.
- [x] **[Introducing Qodo 2.0](https://www.qodo.ai/blog/introducing-qodo-2-0-agentic-code-review/)** (Qodo, 2026-02), found 2026-10-12 (from: bureau-code-review). Specialist agents plus a judge agent, with a benchmark F1 score.
- [x] **[Why code review needs its own AI](https://www.qodo.ai/blog/why-code-review-needs-its-own-ai-with-state-of-the-art-precision-recall/)** (Qodo, 2026), found 2026-10-12 (from: bureau-code-review). Precision and recall argument for a dedicated review model.
- [x] **[How we built Ellipsis](https://www.nsbradford.com/blog/how-we-built-ellipsis)** (Nick Bradford, 2025-01), found 2026-10-12 (from: bureau-code-review). Parallel generators followed by confidence, dedupe and evidence-checking filters.

## Papers

- [x] **[Automated Code Review In Practice](https://arxiv.org/abs/2412.18531)** (arXiv 2412.18531, ICSE SEIP 2025), found 2026-10-12 (from: bureau-code-review). Industry study of LLM review with PR-Agent in production.
- [x] **[Google AutoCommenter](https://arxiv.org/abs/2405.13565)** (arXiv 2405.13565, 2024-05), found 2026-10-12 (from: bureau-code-review). Best-practice comments with per-practice thresholds and no comments on unmodified lines.
- [x] **[Meta RADAR](https://arxiv.org/abs/2605.30208)** (arXiv 2605.30208, 2026-05), found 2026-10-12 (from: bureau-code-review). The one automerge-at-scale system found: risk gating, an LLM safe-category check and delayed landing.
- [x] **[Atlassian RovoDev Code Reviewer](https://arxiv.org/abs/2601.01129)** (arXiv 2601.01129, 2026-01), found 2026-10-12 (from: bureau-code-review). One generator plus a binary judge and an actionability filter, compared with human comments.
- [x] **[ByteDance BitsAI-CR](https://arxiv.org/abs/2501.15134)** (arXiv 2501.15134, FSE 2025), found 2026-10-12 (from: bureau-code-review). Rule checker plus a fine-tuned review filter with production precision numbers.
- [x] **[From Industry Claims to Empirical Reality](https://arxiv.org/abs/2604.03196)** (arXiv 2604.03196, MSR 2026), found 2026-10-12 (from: bureau-code-review). PRs reviewed only by AI agents merge less often than vendor claims suggest.
- [x] **[Does AI Code Review Lead to Code Changes?](https://arxiv.org/abs/2508.18771)** (arXiv 2508.18771, TSE 2026), found 2026-10-12 (from: bureau-code-review). Empirical study of whether AI review comments get acted on.
- [x] **[AI-to-AI Code Reviews of GitHub Pull Requests](https://arxiv.org/abs/2608.21311)** (arXiv 2608.21311, 2026-08), found 2026-10-12 (from: bureau-code-review). Study of AI agents reviewing AI-authored PRs.
