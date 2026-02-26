# Shopizmo Engineering Standards

## 1) Branch Strategy
- `main`: always releasable
- Work happens on feature branches and is merged via Pull Request.

**Branch naming**
- `feat/<short-description>`
- `fix/<short-description>`
- `chore/<short-description>`
Examples:
- `feat/auth-login`
- `fix/payment-webhook`
- `chore/update-deps`

## 2) Commit Message Standard (Conventional Commits)
Use the format:

`type(scope): summary`

**Types**
- `feat`: new feature
- `fix`: bug fix
- `chore`: maintenance / tooling
- `refactor`: code change that neither fixes a bug nor adds a feature
- `docs`: documentation only
- `test`: adding or correcting tests
- `ci`: CI/CD changes

**Examples**
- `feat(auth): add password reset flow`
- `fix(api): handle null customerId`
- `chore(deps): bump next to 14.2`
- `docs(readme): update setup steps`

## 3) Pull Request Rules
- PR title should follow Conventional Commits: `type(scope): summary`
- Keep PRs small and focused
- No secrets in code (keys, passwords, tokens)

## 4) Code Review (when team grows)
- At least 1 approval for customer repos
- CI must pass before merge (enable later)

## 5) Repository Structure (recommended)
- `/docs` for documentation
- `/scripts` for automation
- `.env.example` for environment variables
- `README.md` with setup, run, deploy steps
