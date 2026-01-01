# Contributing to Shelfarr

Thank you for your interest in contributing to Shelfarr! This document provides guidelines and information for contributors.

## How to Contribute

### Reporting Bugs

Before creating a bug report, please check existing issues to avoid duplicates. When creating a bug report, include:

- A clear, descriptive title
- Steps to reproduce the issue
- Expected behavior vs. actual behavior
- Your environment (OS, Ruby version, Docker version if applicable)
- Relevant logs or error messages

### Suggesting Features

Feature requests are welcome! Please:

- Check existing issues and discussions first
- Describe the problem your feature would solve
- Explain your proposed solution
- Consider how it fits with the project's scope (book/audiobook acquisition for Audiobookshelf)

### Pull Requests

1. **Fork the repository** and create your branch from `main`
2. **Set up your development environment:**
   ```bash
   rbenv install 3.3.6
   bundle install
   bin/rails db:setup
   ```
3. **Make your changes** with clear, focused commits
4. **Add tests** for new functionality
5. **Run the test suite:** `bin/rails test`
6. **Update documentation** if needed
7. **Submit your PR** with a clear description of the changes

### Code Style

- Follow existing code patterns and conventions
- Use Ruby community style guidelines
- Keep controllers thin, models focused
- Write clear commit messages

### Development Setup

```bash
# Install dependencies
bundle install

# Set up database
bin/rails db:setup

# Run development server
bin/dev

# Run tests
bin/rails test

# Run background jobs (separate terminal)
bin/jobs
```

### Testing

- Write tests for new features and bug fixes
- Ensure all existing tests pass before submitting a PR
- Use Minitest (Rails default)

## Project Structure

See `CLAUDE.md` for detailed project architecture and patterns.

## Questions?

Feel free to open a discussion or issue if you have questions about contributing.

## License

By contributing to Shelfarr, you agree that your contributions will be licensed under the GPL-3.0 License.
