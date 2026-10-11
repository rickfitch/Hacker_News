# Hacker News Daily AI Briefing

An automated curation and summarization pipeline that monitors the Hacker News front page for breaking breakthroughs, research publications, and community discussions strictly related to **Artificial Intelligence (AI)**, **Large Language Models (LLMs)**, and **Machine Learning (ML)**.

---

## 📌 Project Overview

Hacker News (`news.ycombinator.com`) is one of the highest-signal sources for emerging software developments, scientific breakthroughs, and technical discussions. However, staying up to date can be overwhelming given the high volume of daily posts.

This project extracts, filters, and condenses top-performing AI/ML stories published within a 24-hour window into concise, actionable briefings.

---

## 🎯 Filtering & Curation Rules

The briefing system strictly follows four core rules:

1. **Recency Window**: Scans stories published today or within the last 24 hours.
2. **Strict Domain Focus**: Only extracts and analyzes stories focused directly on AI, LLMs, or machine learning (e.g., model architectures, AI reasoning, evaluation, deployment, or speech synthesis).
3. **No Commercial Distractions**: Automatically filters out job listings (e.g., Y Combinator hiring posts), sponsored posts, and direct advertisements.
4. **Brevity Constraint**: Produces concise summaries strictly **under three sentences** per story, capturing the core contribution, findings, and technical significance.

---

## 📁 Repository Structure

```text
├── AI-News.txt       # The generated daily briefing containing the top 5 curated summaries
└── README.md         # Project documentation and guidelines
```

---

## 📝 Output Details (`AI-News.txt`)

Each briefing entry includes:
- **Story Title**: Name of the article or project.
- **Source Link**: Direct link to the original research paper, slide deck, or website.
- **Discussion Thread**: Direct link to the active Hacker News discussion.
- **Summary**: A two-sentence summary focused on technical takeaways and real-world implications.

### Featured Stories in the Latest Briefing:
1. **Terence Tao: Math 2.0** — Exploration of formal proof systems and AI models revolutionizing mathematical research.
2. **I'm Sorry, But You Still Have to Think** — The architectural and critical-thinking necessities of software engineering in the era of AI coding agents.
3. **BetterWispr** — High-performance, open-source macOS dictation utilizing local speech models (Whisper / Parakeet v3).
4. **Build Your Own Decision Model** — Designing small, fast, deterministic machine learning classifiers over heavy chat LLMs.
5. **Retrofitting Language Models to Operate Over Bytes** — Nature paper exploring token-free language models operating directly on byte streams to eliminate tokenizer errors.

---

## 🚀 How to Run & Automate

The briefing can be refreshed on demand or scheduled as an automated cron task:
- Can be paired with the `/schedule` command or a cron job to generate a fresh `AI-News.txt` daily.
- Supports export to Markdown, plain text, Slack/Discord webhooks, or email digests.
