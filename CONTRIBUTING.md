# Contributing to gamesung

Thank you for your interest in contributing to gamesung! This document provides guidelines and steps for contributing.

## How to Contribute

### 1. Fork the Repository

Click the **Fork** button at the top right of the [repository page](https://github.com/rekabytes/gamesung) to create your own copy.

### 2. Clone Your Fork

```bash
git clone https://github.com/<your-username>/gamesung.git
cd gamesung
```

### 3. Set Up Remote

```bash
git remote add upstream https://github.com/rekabytes/gamesung.git
git remote -v
```

### 4. Create a Branch

Always create a new branch from `dev` for your changes. Use a descriptive name following this convention:

```bash
git checkout dev
git pull upstream dev
git checkout -b <type>/<short-description>
```

**Branch naming:**

| Prefix | Purpose |
|--------|---------|
| `feature/` | New functionality |
| `fix/` | Bug fixes |
| `docs/` | Documentation changes |
| `refactor/` | Code restructuring without behavior changes |
| `test/` | Adding or updating tests |

**Examples:**
- `feature/add-timeout-chess`
- `fix/bot-move-validation`
- `docs/update-api-reference`

### 5. Make Your Changes

- Follow the existing code style
- Keep commits small and focused
- Write clear commit messages

### 6. Commit

```bash
git add .
git commit -m "type: short description

Optional longer description explaining the change."
```

**Commit message format:**
- `feat:` — new feature
- `fix:` — bug fix
- `docs:` — documentation
- `refactor:` — code refactor
- `test:` — adding tests
- `chore:` — maintenance tasks

### 7. Push to Your Fork

```bash
git push origin <your-branch>
```

### 8. Create a Pull Request

1. Go to the original repository
2. Click **New Pull Request**
3. Select `dev` as the base branch
4. Select your branch as the compare branch
5. Fill in the PR template:
   - **Title:** Clear, concise description
   - **Description:** What changed and why
   - **Related Issue:** Link to the issue (if any)

## Pull Request Guidelines

- One feature/fix per PR
- PR should target the `dev` branch, not `main`
- Keep PRs small and focused
- Describe what you changed and why
- Reference any related issues
- Ensure the build passes before submitting

## Code Style

### TypeScript/React (Frontend)
- Use TypeScript for all new files
- Follow existing component patterns
- Use functional components with hooks

### Go (Backend)
- Follow standard Go conventions
- Use `gofmt` for formatting
- Add comments for exported functions

## Issues

- Check existing issues before creating a new one
- Use clear, descriptive titles
- Include steps to reproduce for bugs
- Label issues appropriately

## Code of Conduct

- Be respectful and inclusive
- Welcome newcomers
- Focus on constructive feedback
- No harassment or discrimination

## Questions?

Open an issue with the label `question` if you need help.
