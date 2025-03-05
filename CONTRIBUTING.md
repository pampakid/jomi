# Contributing to Jomi

Thank you for your interest in contributing to Jomi! This document outlines our development workflow and guidelines.

## Git Workflow

We follow a Git Flow-inspired workflow with the following branches:

- `main`: Production-ready code
- `dev`: Development branch for integrating features
- Feature branches: For new features and improvements
- Bug fix branches: For fixing bugs
- Chore branches: For maintenance tasks

### Branch Naming Convention

All branches should follow this naming convention:
- Feature branches: `feat/description`
- Bug fix branches: `fix/description`
- Chore branches: `chore/description`
- Documentation branches: `docs/description`
- Style branches: `style/description`
- Refactor branches: `refactor/description`
- Test branches: `test/description`
- Performance branches: `perf/description`

Examples:
- `feat/user-auth`
- `fix/login-validation`
- `chore/update-dependencies`
- `docs/api-documentation`

### Development Process

1. Create a new branch from `dev`:
   ```bash
   git checkout dev
   git pull origin dev
   git checkout -b feat/your-feature-name
   ```

2. Make your changes and commit following the conventional commits format:
   ```bash
   git commit -m "feat(auth): add login functionality"
   ```

3. Push your branch and create a pull request to `dev`

4. After review and approval, merge into `dev`

5. Once `dev` is stable, create a pull request to `main`

### Commit Message Format

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification:

```
<type>(<scope>): <description>

[optional body]

[optional footer(s)]
```

Types:
- `feat`: New feature
- `fix`: Bug fix
- `chore`: Maintenance tasks
- `docs`: Documentation changes
- `style`: Code style changes
- `refactor`: Code refactoring
- `test`: Adding or modifying tests
- `perf`: Performance improvements

Examples:
```
feat(auth): add login functionality
fix(api): handle null response in user endpoint
chore(deps): update dependencies to latest versions
```

### Pull Request Process

1. Create a pull request using the provided template
2. Ensure all tests pass
3. Get at least one code review
4. Address any feedback
5. Merge only after approval

### Branch Protection Rules

- `main` and `dev` branches are protected
- Direct pushes to `main` and `dev` are not allowed
- All pull requests must pass CI checks
- All pull requests must have at least one approval
- Branch must be up to date before merging

## Code Style

- Follow the existing code style in each component
- Use meaningful variable and function names
- Add comments for complex logic
- Keep functions small and focused
- Write tests for new features

## Testing

- Write unit tests for new features
- Ensure all tests pass before submitting PRs
- Include integration tests for API changes
- Test on both iOS and Android for mobile changes

## Documentation

- Update documentation for any API changes
- Add comments for complex logic
- Update README if needed
- Document any new environment variables

Thank you for contributing to Jomi! 