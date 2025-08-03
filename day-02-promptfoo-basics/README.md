# Day 2 – Getting Productive with **Promptfoo**

Welcome to Day 2 of **How to Test AI Apps**.  
Yesterday you explored common failure modes of LLMs; today you’ll learn how to **codify those checks in Promptfoo** so tests run automatically.

---

## 0  📦 Install Promptfoo

Pick **one** of the methods below (all give the same CLI):

| Package manager | Command |
|-----------------|---------|
| **npm** (global) | `npm install -g promptfoo` |
| **npx** (one-shot) | `npx promptfoo@latest` |
| **Homebrew** | `brew install promptfoo` |

Verify it works:

```bash
promptfoo --version
```

---

## 1  🎯 Prompts

Learn how Promptfoo sources and expands prompts.

| Topic | Goal |
|-------|------|
| **Text prompts** | One-liner prompts in the config file |
| **Multiline prompts** | Use the `|` block syntax for long instructions |
| **Variable prompts** | Inject `${variable}` placeholders at runtime |
| **File-based prompts** | Keep large prompts in separate `.prompt` / `.md` files |


---

## 2  🔌 Providers

Connect Promptfoo to models.

| Topic | What you’ll practice |
|-------|----------------------|
| **Configuration** | Set `OPENAI_API_KEY`, `ANTHROPIC_API_KEY`, etc., via `providers:` block or env vars |
| **Local model** | Point a provider at an **LM Studio** endpoint running on your laptop |



---

## 3  📏 Assertions & Metrics

Automate pass/fail judgment.

### 3.1 Deterministic Assertions  
*Exact string rules.*

| Assertion | Purpose |
|-----------|---------|
| `contains` | Output must include a keyword/phrase |
| `regex` | Output must match a regular expression |

### 3.2 Model-graded Metrics  
*Let an LLM grade another LLM.*

| Metric | Checks |
|--------|--------|
| `answer-relevance` | Does the answer stay on topic? |
| `factuality` | Is the answer factually correct? |
| `llm-rubric` | Custom rubric you provide in prose |


---

Happy testing! 🚀
