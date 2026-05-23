# Contributing to Arc Micro-Yield

We love your input! We want to make contributing to Arc Micro-Yield as easy and transparent as possible.

## Code of Conduct

We are committed to providing a welcoming and inclusive environment. Please be respectful and constructive in all interactions.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, check the issue list as you might find out that you don't need to create one. When you are creating a bug report, include as many details as possible:

* **Use a clear and descriptive title**
* **Describe the exact steps which reproduce the problem**
* **Provide specific examples to demonstrate the steps**
* **Describe the behavior you observed after following the steps**
* **Explain which behavior you expected to see instead and why**
* **Include stack traces if applicable**

### Suggesting Enhancements

When suggesting an enhancement, include:

* **Use a clear and descriptive title**
* **Provide a step-by-step description of the suggested enhancement**
* **Provide specific examples to demonstrate the steps**
* **Describe the current behavior and expected behavior**
* **Explain why this enhancement would be useful**

### Pull Requests

* Fill in the required PR template
* Follow the Dart/Solidity style guides
* Include appropriate test cases
* Update documentation as needed
* End all files with a newline

## Development Process

### Setting Up Your Development Environment

1. Fork the repository
2. Clone your fork
3. Create a feature branch
4. Set up the appropriate development environment

**For Smart Contracts:**
```bash
cd contracts
forge test
```

**For Flutter App:**
```bash
cd app
flutter pub get
flutter run
```

### Making Changes

1. Create a descriptive branch name: `feature/user-auth` or `fix/deposit-bug`
2. Make your changes
3. Add tests for new functionality
4. Ensure all tests pass
5. Update documentation if needed

### Commit Guidelines

Use clear and descriptive commit messages:

```
feat: Add user authentication
fix: Resolve deposit calculation bug
docs: Update API documentation
test: Add tests for yield distribution
refactor: Simplify strategy selection
style: Format code according to guidelines
```

### Testing

**Smart Contracts:**
```bash
cd contracts
forge test -v                    # Run all tests
forge test -v --match YieldTest # Run specific test
forge analyze                    # Code analysis
```

**Flutter App:**
```bash
cd app
flutter test                     # Run tests
flutter analyze                  # Code analysis
flutter format lib/              # Format code
```

## Style Guides

### Solidity

* Follow [Solidity Style Guide](https://docs.soliditylang.org/en/latest/style-guide.html)
* Use OpenZeppelin library conventions
* Maximum line length: 120 characters
* Comment all public functions
* Use descriptive variable names

### Dart/Flutter

* Follow [Dart Style Guide](https://dart.dev/guides/language/effective-dart/style)
* Use `flutter format` before committing
* Maximum line length: 100 characters
* Document public APIs
* Use meaningful variable names

### Documentation

* Use clear, concise language
* Include code examples where applicable
* Keep documentation up-to-date with code changes
* Use markdown formatting

## Pull Request Process

1. Update README.md with any new features or changes
2. Increase version numbers following [Semantic Versioning](https://semver.org/)
3. Ensure all tests pass
4. Ensure code analysis shows no errors
5. Request review from maintainers
6. Address any feedback
7. Merge after approval

## Additional Notes

### Issue and Pull Request Labels

* `bug` - Something isn't working
* `enhancement` - New feature or request
* `documentation` - Improvements or additions to documentation
* `good first issue` - Good for newcomers
* `help wanted` - Extra attention is needed
* `question` - Further information is requested

## Community

* Follow the Code of Conduct
* Be respectful and inclusive
* Help others in the community
* Share knowledge and best practices

## Questions?

Don't hesitate to ask for help:

* Open a GitHub discussion
* Check existing documentation
* Review similar code
* Ask in issues or PRs

## Recognition

Contributors will be recognized in:
* CONTRIBUTORS.md file
* GitHub contributors page
* Project documentation

Thank you for contributing to Arc Micro-Yield! 🈀
