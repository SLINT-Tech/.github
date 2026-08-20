# Contributing to SLINT Tech

Thank you for wanting to build with us.

This guide covers every repository in the [@SLINT-Tech](https://github.com/SLINT-Tech)
organization. A repository may add its own `CONTRIBUTING.md` with extra detail — where it does,
that one wins.

**Everyone who contributes agrees to our [Code of Conduct](CODE_OF_CONDUCT.md).**

## New to this? Start here

You do not need experience to contribute. Many of our members write their first pull request
here, and that is the point.

1. Look for issues labelled **`good first issue`** — they are scoped small on purpose.
2. Comment on the issue saying you would like to take it, so two people don't do the same work.
3. Ask questions in the issue. Asking is not a weakness; guessing silently is.
4. Your Cell Leader can pair with you on your first one.

## The workflow

### 1. Get the code

Members of a cell can push branches directly to that cell's repositories. Everyone else forks.

```bash
git clone https://github.com/SLINT-Tech/<repository>.git
cd <repository>
git checkout -b feat/short-description
```

### 2. Branch naming

| Prefix | Use for |
| --- | --- |
| `feat/` | A new feature |
| `fix/` | A bug fix |
| `docs/` | Documentation only |
| `refactor/` | Restructuring without behaviour change |
| `chore/` | Tooling, dependencies, config |

Example: `feat/member-signup-form`, `fix/broken-nav-on-mobile`

### 3. Commit messages

We use [Conventional Commits](https://www.conventionalcommits.org). One logical change per commit.

```
feat(signup): validate phone number before submit

The form accepted malformed numbers, which broke the SMS confirmation.
Adds Ghana-format validation and an inline error message.

Closes #42
```

Write the subject line in the imperative — "add", not "added" — and keep it under 72 characters.

### 4. Before you open a pull request

- [ ] The project builds and runs locally
- [ ] Tests pass, and you added tests for behaviour you changed
- [ ] Linter and formatter are clean
- [ ] **No secrets, API keys, `.env` files, or personal data are in the diff**
- [ ] You updated the docs if you changed how something works

### 5. Open the pull request

Fill in the template. A good pull request explains **why**, not just what — the diff already shows
what. Link the issue it closes. If it changes anything visual, include a screenshot.

Keep pull requests small. A 200-line pull request gets reviewed today; a 2,000-line one waits a
week and gets a worse review.

### 6. Review

- At least one maintainer approval is required to merge.
- Reviewers respond within **five (5) business days**. Nudge us if we go quiet.
- Review comments are about the code, never the person. If a comment ever feels otherwise,
  report it under the [Code of Conduct](CODE_OF_CONDUCT.md).
- Push follow-up commits to the same branch; do not force-push once review has started.

## Security

Never open a public issue or pull request for a security vulnerability — follow
[SECURITY.md](SECURITY.md).

If you accidentally commit a credential, tell us at
[security@slinttech.org](mailto:security@slinttech.org) straight away. Removing the commit does not
undo the exposure; the credential has to be rotated. Reporting fast is never punished.

## Licensing and ownership

By contributing, you agree your contribution is licensed under the same licence as the repository
you are contributing to, and you confirm you have the right to submit it.

Do not paste code you do not have the right to share — from an employer, a paid course, or a
tutorial with a restrictive licence. When you adapt something, credit the source in a comment.

## Using AI assistants

You may use AI coding tools. You remain responsible for every line you submit: understand it,
test it, and be able to explain it in review. Do not paste SLINT Tech private data or credentials
into a third-party tool.

## Attribution

Contributors are credited in release notes. Sustained contribution is one of the paths to a Cell
Leader or maintainer role.

---

*Questions: [support@slinttech.org](mailto:support@slinttech.org) · Program questions:
[programs@slinttech.org](mailto:programs@slinttech.org)*
