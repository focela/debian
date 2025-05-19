# Contributing to docker-debian

## Overview

Thank you for your interest in contributing to the docker-debian project! This guide outlines the process for contributing and the standards we expect contributors to follow.

We welcome contributions of all kinds:
- Code improvements
- Bug fixes
- Documentation updates
- Feature additions
- Performance enhancements

## Contribution Workflow

### 1. Prepare Your Development Environment

#### Fork and Clone the Repository

```bash
# Create your own fork of the repository
# Go to https://github.com/focela/docker-debian and click "Fork"

# Clone your fork locally
git clone https://github.com/<your-username>/docker-debian.git
cd docker-debian

# Add the upstream repository for synchronization
git remote add upstream https://github.com/focela/docker-debian.git
```

#### Stay Updated

```bash
# Fetch the latest changes from upstream
git fetch upstream

# Merge upstream changes into your local main branch
git checkout main
git merge upstream/main
```

### 2. Plan Your Contribution

- For bug fixes: Verify the bug exists and can be reproduced
- For features: Consider the scope and alignment with project goals
- For documentation: Identify areas that need clarification or updates

#### Create a Focused Branch

```bash
# Use a descriptive branch name based on the type of change
# Format: <type>/<description>
# Examples:
git checkout -b feat/add-msmtp-support
git checkout -b fix/zabbix-agent-startup
git checkout -b docs/improve-environment-variables
```

### 3. Implement Your Changes

#### Code Style Guidelines

- Follow the existing code style and formatting
- Keep the Dockerfile clean, organized, and well-commented
- Use meaningful variable names and add comments for complex logic
- Maintain backward compatibility where possible

#### Documentation Standards

- Update any relevant documentation affected by your changes
- Document new features thoroughly
- Include examples for non-trivial functionality

### 4. Verify Your Changes

#### Testing Requirements

```bash
# Build a test image with your changes
docker build -t test-debian-image .

# Run the container to verify functionality
docker run --rm test-debian-image

# Optional: Run with specific environment variables to test features
docker run --rm -e DEBUG_MODE=TRUE test-debian-image
```

- Ensure your changes don't break existing functionality
- If adding features, consider adding example usage in documentation
- Test on multiple architectures if possible (amd64, arm64, etc.)

### 5. Commit Your Changes

#### Conventional Commits Format

We use the [Conventional Commits](https://www.conventionalcommits.org/) standard:

```
<type>(<scope>): <description>

[optional body]

[optional footer(s)]
```

Examples:
```
feat(monitoring): add Zabbix agent 2 support

fix(s6): resolve service startup ordering issue

docs(env): clarify environment variable descriptions
```

**Types:**
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Formatting changes
- `refactor`: Code changes that neither fix bugs nor add features
- `perf`: Performance improvements
- `test`: Adding/modifying tests
- `chore`: Maintenance tasks, dependency updates, etc.

**Important Notes:**
- Use English for commit messages
- Keep the subject line concise (50 characters max)
- Use the imperative mood ("Add feature" not "Added feature")
- Reference issues in the footer when applicable

### 6. Submit a Pull Request

1. Push your branch to your fork:
   ```bash
   git push origin <your-branch-name>
   ```

2. Create a pull request:
    - Go to the [docker-debian repository](https://github.com/focela/docker-debian)
    - Click "New Pull Request"
    - Select "compare across forks"
    - Select your fork and branch

3. Fill out the pull request template with:
    - A clear title following conventional commits format
    - A detailed description of the changes
    - Any breaking changes or dependencies
    - References to related issues

4. Await review from maintainers

## Additional Guidelines

### Communication

- Use GitHub Issues to discuss large changes before implementing
- Be respectful and open to feedback
- Ask questions if something is unclear

### Pull Request Size

- Keep pull requests focused on a single change
- Break large changes into smaller, logical pull requests
- This makes review easier and increases the chance of acceptance

### Review Process

- Maintainers will review your PR as soon as possible
- Address review feedback promptly
- Be prepared to make requested changes

### License

By contributing, you agree that your contributions will be licensed under the same license as the project.

## Thank You!

Your contributions help improve docker-debian for everyone. We appreciate the time and effort you put into making this project better!
