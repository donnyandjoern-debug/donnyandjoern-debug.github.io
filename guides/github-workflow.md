# 🔀 GitHub Workflow Guide — Family Hoppe

Best practices for clean, professional GitHub work across all Family Hoppe projects.

---

## Branch Strategy

Use a simple **feature-branch workflow**:

```
main           ← stable, always deployable
└── feature/short-description   ← your working branch
└── fix/issue-description       ← bug fix branch
└── docs/update-readme          ← documentation update
```

**Rules:**
- Never commit directly to `main`
- Branch names: lowercase, hyphens only, descriptive (e.g., `feature/add-user-login`)
- Delete branches after merging

---

## Commit Messages

Follow the **Conventional Commits** format:

```
<type>: <short description>

[optional body]
[optional footer]
```

| Type | When to use |
|---|---|
| `feat:` | A new feature |
| `fix:` | A bug fix |
| `docs:` | Documentation changes only |
| `chore:` | Maintenance (deps, config, cleanup) |
| `refactor:` | Code restructuring without feature/fix |
| `test:` | Adding or updating tests |

**Examples:**
```
feat: add user authentication
fix: correct off-by-one error in pagination
docs: update README with installation steps
chore: update dependencies to latest versions
```

---

## Pull Request Checklist

Before opening a PR:
- [ ] Branch is up to date with `main`
- [ ] All tests pass
- [ ] Code has been reviewed (or Copilot Chat used to review)
- [ ] PR description explains what and why
- [ ] No secrets or credentials in the diff

---

## Issue Best Practices

Write issues that Copilot (and humans) can act on:

1. **Title:** Short and specific (e.g., "Add dark mode toggle to settings page")
2. **Description:** What should happen vs. what currently happens
3. **Acceptance criteria:** Bullet list of what "done" looks like
4. **Labels:** Use labels (`bug`, `feature`, `docs`, `chore`)
5. **Assignee:** Assign to yourself or to Copilot

**Good issue template:**
```markdown
## What
A clear description of the change needed.

## Why
Why is this needed? What problem does it solve?

## Acceptance Criteria
- [ ] Criterion 1
- [ ] Criterion 2

## Additional Context
Any links, screenshots, or related issues.
```

---

## Repo Hygiene

Keep repos clean and professional:

| Practice | Description |
|---|---|
| **README.md** | Every repo needs one — what is it, how to run it |
| **LICENSE** | Add a license (MIT for open source) |
| **.gitignore** | Always add a proper `.gitignore` |
| **Branch protection** | Protect `main` — require PR reviews |
| **Archive old repos** | Don't delete — archive when no longer active |
| **Descriptive names** | `hoppe-home/recipe-manager`, not `test123` |

---

## GitHub Search Shortcuts

| Shortcut | Action |
|---|---|
| `t` | Search files in the current repo |
| `/` | Focus global search |
| `g c` | Go to Code tab |
| `g i` | Go to Issues tab |
| `g p` | Go to Pull Requests tab |
| `?` | Show all keyboard shortcuts |

---

## Useful GitHub CLI Commands

```bash
# Create a new branch and PR
gh pr create --title "feat: my feature" --body "Description here"

# View open PRs
gh pr list

# Check out a PR locally
gh pr checkout <number>

# View open issues
gh issue list

# Create an issue
gh issue create --title "bug: something is broken" --label "bug"

# View repo status
gh repo view
```

---

[← Back to guides](./README.md) | [← Back to main library](../README.md)
