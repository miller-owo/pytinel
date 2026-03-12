# Contributing to Pytinel

🎉 Welcome Contributors!
Thank you for your interest in contributing to the Pytinel project. This document outlines the rigorous standards and procedures required for contribution.

⚠️ **Prerequisite**: Before proceeding, please read the `README.md` thoroughly. It contains essential information regarding project architecture, environment configuration, and feature specifications. This guide focuses exclusively on contribution protocols; it does not duplicate the setup instructions found in the README.

---

## 1. Contribution Avenues

We accept contributions through the following channels:

| Channel | Purpose | Requirements |
|---------|---------|--------------|
| Issues | Report bugs, request features, or discuss architectural changes. | Must follow the Issue Template. |
| Pull Requests (PRs) | Fix bugs, implement features, improve documentation, or refactor code. | Must follow the Development Workflow and Commit Standards. |
| Community Support | Improve test coverage, refine code comments, or enhance translations. | Must align with existing style guides and pass CI checks. |

---

## 2. Issue Specifications

To ensure efficient triage, all issues must adhere to the following structure:

### 🐛 Bug Reports
- **Title**: Must be descriptive and specific (e.g., `[Bug] Memory leak in module X when Y occurs`).
- **Environment**: Specify OS, Python version, and Pytinel version (as defined in `README.md`).
- **Reproduction Steps**: Provide a minimal, reproducible example.
- **Evidence**: Attach relevant logs, stack traces, or screenshots.

### 💡 Feature Requests
- **Title**: Clearly state the proposed functionality.
- **Use Case**: Describe the problem this feature solves and its value proposition.
- **Scope**: Define expected behavior and potential impact on existing systems.

---

## 3. Development Workflow

### 3.1 Pre‑Submission Checklist
Before submitting a Pull Request, you must ensure:

- ✅ The code compiles without errors.
- ✅ All existing unit tests pass locally (`pytest` or equivalent).
- ✅ New features include corresponding test cases.
- ✅ No regression is introduced to existing functionality.
- ✅ Code follows the project’s linting and styling rules.

### 3.2 Pull Request Guidelines
- **Branching**: Create a new branch from `main` (e.g., `feat/add-login`, `fix/memory-leak`).
- **Title**: Use the Conventional Commits format.
- **Description**:
  - Summarize the changes clearly.
  - Link related issues (e.g., `Closes #123`).
  - Explain the rationale behind significant design decisions.
- **Conflict Resolution**: Ensure the branch is rebased against the latest `main` to resolve any merge conflicts prior to review.

---

## 4. Commit Standards

All commits must follow the **Conventional Commits** specification to facilitate automated changelog generation and semantic versioning.

### Format
```
<type>(<scope>): <subject>

<body> (Optional)

<footer> (Optional)
```

### Allowed Types

| Type | Description |
|------|-------------|
| feat | A new feature for the user. |
| fix | A bug fix for the user. |
| docs | Documentation only changes (including README). |
| style | Changes that do not affect the meaning of the code (white‑space, formatting, etc.). |
| refactor | A code change that neither fixes a bug nor adds a feature. |
| test | Adding missing tests or correcting existing tests. |
| chore | Changes to the build process or auxiliary tools (no production code change). |

### Example
```
feat(auth): add OAuth2 support for Google login

Implemented OAuth2 flow to allow users to sign in via Google accounts.
Updated database schema to store provider IDs.

Closes #45
```

---

## 5. Developer Certificate of Origin (DCO)

By contributing to this project, you explicitly agree to the terms of the **Developer Certificate of Origin (Version 1.1)**. This certifies that:

- The contribution was created in whole or in part by you, and you have the right to submit it.
- OR the contribution is based upon previous work that, to the best of your knowledge, is covered under an appropriate open‑source license.
- You understand and agree that this project and the contribution are public and that a record of the contribution (including all personal information you submit with it) is maintained indefinitely.

### How to Sign Off

Every commit message must contain a `Signed-off-by` line. Use the `-s` flag with Git:

```bash
git commit -s -m "feat: implement new parser"
```

This automatically appends:
```
Signed-off-by: Your Name <your.email@example.com>
```

**Note**: The email address must match the one associated with your GitHub account and must be valid for verification purposes. PRs without a valid DCO sign‑off will not be merged.

---

## 6. Code of Conduct

We are committed to providing a welcoming and inspiring community for all.

- **Respect**: Treat all contributors with respect and courtesy.
- **Inclusivity**: Embrace diverse perspectives and backgrounds.
- **Professionalism**: Refrain from offensive, irrelevant, or harassing language.
- **Constructive Feedback**: Focus on technical merit rather than personal attributes.

Violations of this code may result in temporary or permanent bans from the project community.

---

## 7. Acknowledgments

We sincerely appreciate every contribution, regardless of size. Your efforts drive the growth and success of Pytinel.

If you have questions or need assistance:
- Open a discussion in the Issues tab.
- Check the Discussions area for community support.
- Refer to the contact channels listed in the `README.md`.

Thank you for making Pytinel better! 🚀