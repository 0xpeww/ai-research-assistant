# AI Research Assistant

> Autonomous research agent that reads papers, extracts insights, generates summaries, and proposes experiments.

## 🎯 What It Solves

Researchers spend 40% of their time just reading and synthesizing literature. This agent automates literature review, hypothesis generation, and experimental design — allowing researchers to focus on actual experimentation.

## 🏗️ Architecture

```
Topic/Query → Search Agent → Paper Fetcher → [Summarizer | Critic | Synthesizer]
                                                ↓
                                    Insight Database → Report Generator
```

## 🔧 Core Features

- **Paper Fetcher**: Downloads from arXiv, PubMed, Semantic Scholar APIs
- **Summarizer Agent**: Extracts key contributions, methods, results
- **Critic Agent**: Identifies methodological flaws, reproducibility issues
- **Synthesizer Agent**: Cross-references findings, identifies contradictions
- **Experiment Designer**: Suggests next experiments based on gaps

## 📊 Token Consumption

- Single paper analysis: ~20K tokens
- Literature review (50 papers): ~800K tokens
- Weekly research digest: ~200K tokens
- **Monthly average**: 5-10M tokens for active research group

## 🚀 Quick Start

```bash
pip install -r requirements.txt
python research.py --topic "transformer efficiency optimization" --papers 30
```

## 📈 Results

Used by a university NLP lab:
- Literature review time: 2 weeks → 2 days
- Discovered 7 overlooked papers relevant to their work
- Generated 3 novel experiment proposals (1 led to publication)

## 🛠️ Tech Stack

- Python 3.11+
- MiMo API + Claude Code
- arXiv API, Semantic Scholar API
- Pinecone for vector storage
