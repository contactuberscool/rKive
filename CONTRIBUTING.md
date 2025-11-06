# Contributing to rKive

Thank you for your interest in contributing to rKive! This document provides guidelines and instructions for collaborating on this project.

## Getting Started

### Prerequisites

- Git installed on your machine
- A GitHub account
- Access to the repository (you'll need to be added as a collaborator)

### Setting Up Your Development Environment

1. **Fork or Clone the Repository:**
   ```bash
   git clone https://github.com/contactuberscool/rKive.git
   cd rKive
   ```

2. **Verify the Setup:**
   ```bash
   git remote -v
   # Should show: origin  https://github.com/contactuberscool/rKive.git
   ```

## Collaboration Workflow

### 1. Create a Branch

Always create a new branch for your work. Never commit directly to `main`.

```bash
# Update your local main branch
git checkout main
git pull origin main

# Create a new branch for your feature
git checkout -b feature/your-feature-name
# Or for bug fixes:
git checkout -b fix/issue-description
```

**Branch Naming Conventions:**
- `feature/` - For new features
- `fix/` - For bug fixes
- `docs/` - For documentation updates
- `refactor/` - For code refactoring
- `test/` - For adding tests

### 2. Make Your Changes

- Write clear, readable code
- Follow existing code style
- Add comments where necessary
- Test your changes locally

### 3. Commit Your Changes

```bash
# Stage your changes
git add .

# Commit with a descriptive message
git commit -m "Add feature: description of what you added"
```

**Commit Message Guidelines:**
- Use present tense ("Add feature" not "Added feature")
- Be descriptive and specific
- Keep the first line under 50 characters
- Add more details in the body if needed

### 4. Push Your Branch

```bash
# Push your branch to GitHub
git push origin feature/your-feature-name
```

If this is your first push, Git will provide a command to set the upstream:
```bash
git push --set-upstream origin feature/your-feature-name
```

### 5. Create a Pull Request

1. Go to https://github.com/contactuberscool/rKive
2. You'll see a banner suggesting to create a pull request for your new branch
3. Click "Compare & pull request"
4. Fill out the pull request template:
   - **Title:** Clear description of your changes
   - **Description:** Explain what you changed and why
   - **Screenshots:** If applicable, add screenshots
5. Request review from collaborators
6. Click "Create pull request"

### 6. Review Process

- Collaborators will review your code
- Address any feedback or requested changes
- Update your branch by pushing new commits
- Once approved, a collaborator will merge your PR

### 7. Keep Your Branch Updated

While waiting for review, keep your branch up to date with main:

```bash
# Switch to your branch
git checkout feature/your-feature-name

# Fetch latest changes
git fetch origin

# Merge main into your branch
git merge origin/main

# Or use rebase (cleaner history)
git rebase origin/main

# Push updated branch
git push origin feature/your-feature-name
```

## Best Practices

### Code Quality

- Write clean, readable code
- Follow consistent formatting
- Add comments for complex logic
- Remove unused code

### Communication

- Use clear commit messages
- Write descriptive pull request descriptions
- Respond to review comments promptly
- Ask questions if something is unclear

### Testing

- Test your changes locally before pushing
- Ensure existing functionality still works
- Add tests for new features when possible

### File Organization

- Keep files organized in appropriate directories
- Use meaningful file and folder names
- Don't commit unnecessary files (use .gitignore)

## Common Git Commands

```bash
# Check current status
git status

# View changes
git diff

# View commit history
git log

# Update from remote
git pull origin main

# View branches
git branch -a

# Switch branches
git checkout branch-name

# Delete a branch (after merge)
git branch -d branch-name
```

## Getting Help

If you encounter any issues:

1. Check the README.md for setup instructions
2. Review existing issues on GitHub
3. Ask questions in pull request comments
4. Contact the repository maintainer

## Code of Conduct

- Be respectful and professional
- Provide constructive feedback
- Help others learn and grow
- Focus on the code, not the person

Thank you for contributing to rKive! 🚀
