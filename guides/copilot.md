# 🤖 GitHub Copilot Guide — Family Hoppe

Quick reference for getting the most out of GitHub Copilot across both Family Hoppe accounts.

---

## Accounts & Plans

| Account | Plan | Editor | Status |
|---|---|---|---|
| donnyandjoern-debug | Copilot Pro ($10/mo) | VS Code (Mac) | ✅ Active |
| Joern _(account pending creation)_ | Copilot Pro ($10/mo) | VS Code (Windows) | 🟡 Planned |

---

## Copilot Features (Pro Plan)

| Feature | Description | Where |
|---|---|---|
| **Code completion** | Inline AI suggestions as you type | VS Code editor |
| **Copilot Chat** | Ask questions about code, get explanations | VS Code sidebar / inline |
| **Copilot Edits** | Multi-file AI edits for larger changes | VS Code |
| **Copilot Coding Agent** | Autonomous agent that solves GitHub issues | GitHub.com (browser) |
| **PR summaries** | Auto-generated pull request descriptions | GitHub.com |
| **Copilot CLI** | AI-powered terminal suggestions | Terminal / shell |
| **GitHub Models** | Access to AI models via the API | GitHub Marketplace |

---

## VS Code Setup

### Install Copilot in VS Code

1. Open VS Code
2. Go to Extensions (`Ctrl+Shift+X` / `Cmd+Shift+X`)
3. Search for **"GitHub Copilot"** and install it
4. Also install **"GitHub Copilot Chat"**
5. Sign in with your GitHub account when prompted

### Key Shortcuts (VS Code)

| Action | Mac | Windows |
|---|---|---|
| Accept suggestion | `Tab` | `Tab` |
| Dismiss suggestion | `Esc` | `Esc` |
| Next suggestion | `Alt+]` | `Alt+]` |
| Previous suggestion | `Alt+[` | `Alt+[` |
| Open Copilot Chat | `Ctrl+Cmd+I` | `Ctrl+Alt+I` |
| Inline chat | `Cmd+I` | `Ctrl+I` |
| Open Copilot Edits | `Ctrl+Shift+I` | `Ctrl+Shift+I` |

---

## Copilot Coding Agent (Cloud Agent)

The Copilot Coding Agent lets Copilot autonomously work on GitHub issues:

1. Go to a GitHub Issue in your browser
2. Click **"Assign to Copilot"** (or mention `@github-copilot` in a comment)
3. Copilot opens a PR with the solution
4. Review the PR, request changes if needed, and merge

**Tips:**
- Write clear, detailed issue descriptions — the agent works from the issue text.
- The agent works best on well-scoped, single-concern issues.
- Always review the agent's PR before merging.

---

## Multi-Account Workflow

When working across both accounts (Mac + Windows):

1. Each account has its own Copilot Pro subscription — they work independently.
2. Both accounts can collaborate on the same Hoppe-home organisation repos.
3. Copilot suggestions are personal — they do not sync between accounts.
4. Use GitHub Issues and PRs to hand off work between accounts.

---

## Useful Copilot Chat Prompts

```
# Explain code
/explain

# Fix a bug
/fix

# Generate tests
/tests

# Create documentation
/doc

# Simplify code
Simplify this function and reduce duplication

# Review a PR
Review this pull request for security issues and code quality

# Clean up a repo
What files in this repo are redundant or should be removed?
```

---

## Best Practices

- ✅ Always review Copilot suggestions before accepting
- ✅ Use Copilot Chat to understand unfamiliar code
- ✅ Use the Coding Agent for well-defined GitHub issues
- ✅ Write good commit messages — Copilot can help with these too
- ❌ Don't accept suggestions blindly — Copilot can hallucinate
- ❌ Don't use Copilot to generate secrets, passwords, or credentials

---

[← Back to guides](./README.md) | [← Back to main library](../README.md)
