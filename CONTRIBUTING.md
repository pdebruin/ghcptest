# Contributing to ghcptest

Thank you for your interest in contributing to ghcptest! This document provides guidelines and instructions for contributing.

## Code of Conduct

This project adheres to a Code of Conduct that all contributors are expected to follow. Please read [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) before contributing.

## How to Contribute

### Reporting Issues

- Check if the issue already exists before creating a new one
- Provide a clear and descriptive title
- Include steps to reproduce the issue
- Describe the expected behavior and actual behavior
- Include relevant logs, screenshots, or code snippets

### Submitting Pull Requests

1. Fork the repository
2. Create a new branch for your feature or bug fix (`git checkout -b feature/your-feature-name`)
3. Make your changes following the code style guidelines
4. Write or update tests as needed
5. Ensure all tests pass
6. Commit your changes with clear, descriptive messages
7. Push to your fork and submit a pull request

## Code Style Guidelines

- Follow clean code principles
- Write clear and descriptive commit messages
- Keep functions small and focused
- Use meaningful variable and function names
- Document complex logic with comments

## Testing Guidelines

- Write tests for new features
- Ensure all tests pass before committing
- Aim for high code coverage
- Test edge cases

## Documentation

- Update README.md when adding new features
- Document complex logic with comments
- Keep documentation up to date with code changes

## Best Practices

- Make small, incremental changes
- Review code before committing
- Follow existing code patterns and conventions
- Consider edge cases when implementing features

## Questions?

Feel free to open an issue for any questions or concerns.
Thank you for your interest in contributing to ghcptest! This document provides guidelines and instructions for contributing to this project.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Guidelines](#development-guidelines)
- [Code Style Guidelines](#code-style-guidelines)
- [Testing Guidelines](#testing-guidelines)
- [Pull Request Process](#pull-request-process)
- [Reporting Issues](#reporting-issues)

## Code of Conduct

This project and everyone participating in it is governed by our commitment to creating a welcoming and inclusive environment. Please be respectful and constructive in all interactions.

## How Can I Contribute?

### Reporting Bugs

If you find a bug, please create an issue with:
- A clear and descriptive title
- Steps to reproduce the issue
- Expected behavior vs. actual behavior
- Any relevant logs or screenshots
- Your environment details (OS, version, etc.)

### Suggesting Enhancements

Enhancement suggestions are welcome! Please create an issue with:
- A clear and descriptive title
- Detailed description of the proposed enhancement
- Explanation of why this enhancement would be useful
- Any relevant examples or mockups

### Contributing Code

1. Fork the repository
2. Create a new branch for your feature or bugfix (`git checkout -b feature/your-feature-name`)
3. Make your changes following our guidelines
4. Test your changes thoroughly
5. Commit your changes with clear commit messages
6. Push to your fork
7. Submit a pull request

## Development Guidelines

### Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/pdebruin/ghcptest.git
   cd ghcptest
   ```

2. Create a new branch for your work:
   ```bash
   git checkout -b feature/your-feature-name
   ```

### Best Practices

- Make small, incremental changes
- Review your code before committing
- Follow existing code patterns and conventions
- Consider edge cases when implementing features
- Keep functions small and focused
- Write self-documenting code with meaningful names

## Code Style Guidelines

Please adhere to the following code style guidelines:

- **Clean Code Principles**: Follow clean code principles in all contributions
- **Naming Conventions**: Use meaningful variable and function names that clearly describe their purpose
- **Function Size**: Keep functions small and focused on a single responsibility
- **Comments**: Document complex logic with clear comments
- **Commit Messages**: Write clear and descriptive commit messages that explain the "why" behind changes

### Commit Message Format

Good commit messages should:
- Use the imperative mood ("Add feature" not "Added feature")
- Be concise but descriptive
- Reference issue numbers when applicable (e.g., "Fix issue #123")

Example:
```
Add user authentication feature

- Implement JWT token validation
- Add login endpoint
- Update user model with password hashing
```

## Testing Guidelines

Testing is crucial to maintaining code quality:

- **Write Tests**: Write tests for new features and bug fixes
- **Run Tests**: Ensure all tests pass before submitting a pull request
- **Coverage**: Aim for high code coverage
- **Test Types**: Include unit tests, integration tests where applicable

Before submitting your pull request, verify that:
```bash
# Run all tests
# (Add specific test commands for this project)
```

## Pull Request Process

1. **Update Documentation**: Ensure relevant documentation is updated, including:
   - README.md for new features
   - Code comments for complex logic
   - Any other relevant documentation

2. **Self-Review**: Review your own code before requesting reviews from others:
   - Check for console.log or debug statements
   - Verify code follows style guidelines
   - Ensure no unrelated changes are included

3. **PR Description**: Provide a clear description of:
   - What changes were made
   - Why the changes were necessary
   - How to test the changes
   - Any breaking changes or migration notes

4. **Respond to Feedback**: Be responsive to review comments and make requested changes promptly

5. **Keep Updated**: Keep your PR up to date with the main branch

## Reporting Issues

When creating an issue:

1. **Search First**: Check if a similar issue already exists
2. **Use Templates**: Use issue templates if available
3. **Be Specific**: Provide as much relevant detail as possible
4. **One Issue Per Report**: Keep issues focused on a single bug or feature
5. **Follow Up**: Respond to questions and provide additional information when requested

## Questions?

If you have questions about contributing, feel free to:
- Open an issue with the "question" label
- Reach out to the maintainers

## Recognition

Contributors who submit pull requests will be recognized in our project. Thank you for helping make this project better!

---

Thank you for contributing to ghcptest! 🎉
