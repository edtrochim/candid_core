# Contributing to the Candid Core Framework

Thank you for your interest in contributing to the Candid Core Framework! This document provides guidelines for contributing to this project and helping to improve geospatial metadata through Data Candor.

## Table of Contents
- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
  - [Reporting Issues](#reporting-issues)
  - [Suggesting Enhancements](#suggesting-enhancements)
  - [Your First Code Contribution](#your-first-code-contribution)
  - [Pull Requests](#pull-requests)
- [Styleguides](#styleguides)
  - [Git Commit Messages](#git-commit-messages)
  - [Documentation Styleguide](#documentation-styleguide)
- [Field Contributions](#field-contributions)
- [Community](#community)

## Code of Conduct

This project and everyone participating in it is governed by our Code of Conduct. By participating, you are expected to uphold this code. Please report unacceptable behavior to [MAINTAINER EMAIL].

## How Can I Contribute?

### Reporting Issues

Found a problem with the framework or documentation? Here's how to report it:

1. **Check Existing Issues** - Search the [issue tracker](https://github.com/your-username/candid-core-framework/issues) to see if your issue has already been reported.

2. **Create a New Issue** - If your issue is unreported, create a new issue with:
   - A clear title describing the issue
   - A detailed description of the problem
   - Steps to reproduce (if applicable)
   - Expected vs. actual behavior
   - Screenshots or examples (if helpful)
   - Your environment info (if relevant)

3. **Use Issue Templates** - Please use the appropriate issue template if available.

### Suggesting Enhancements

Have ideas for improving the Candid Core Framework? We'd love to hear them:

1. **Check Existing Suggestions** - Search the [issue tracker](https://github.com/your-username/candid-core-framework/issues) for similar ideas.

2. **Create an Enhancement Suggestion** - If your idea is new, create an issue with:
   - A clear title describing the enhancement
   - A detailed description of the suggested functionality
   - Rationale: why would this enhancement help users?
   - Any examples from other frameworks or standards that implement similar features
   - Mockups or examples of how the enhancement would work (if applicable)

### Your First Code Contribution

New to contributing? Here are some good starting points:

- **Beginner Issues** - Look for issues labeled "good first issue" or "help wanted"
- **Documentation Improvements** - Fixing typos or clarifying existing documentation
- **Example Additions** - Adding new examples of how to use the framework

### Pull Requests

1. **Fork the Repository** - Fork the project to your GitHub account.

2. **Create a Branch** - Create a branch in your fork for your contribution:
   ```
   git checkout -b feature/your-feature-name
   ```

3. **Make Your Changes** - Implement your changes, following our styleguides.

4. **Submit a Pull Request** - Push your changes to your fork and submit a pull request to our repository.

5. **Review Process** - Your pull request will be reviewed by maintainers who may suggest changes or improvements.

## Styleguides

### Git Commit Messages

- Use the present tense ("Add feature" not "Added feature")
- Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
- Limit the first line to 72 characters or less
- Reference issues and pull requests after the first line
- Consider starting the commit message with an applicable emoji:
  - ✨ `:sparkles:` for new features
  - 🐛 `:bug:` for bug fixes
  - 📝 `:memo:` for documentation
  - 🧹 `:broom:` for code cleanup

### Documentation Styleguide

- Use Markdown for all documentation
- Follow a consistent heading hierarchy
- Include example code in proper code blocks with language specification
- Use links to reference other documents rather than duplicating information
- Check spelling and grammar before submitting

## Field Contributions

When suggesting new fields for the Candid Core Framework:

1. **Check Existing Fields** - Review `schema/candid-core-fields.csv` to ensure your suggestion isn't already covered.

2. **Field Definition** - Provide:
   - Field name (in snake_case)
   - Clear description
   - Category it belongs to
   - Example values
   - Whether it should be required or optional
   - Rationale for why this field enhances Data Candor

3. **Example Implementation** - Show how your field would be used in a real-world example.

## Community

- **Join the Discussion** - Participate in discussions in the repository's Discussions tab
- **Share Your Implementation** - If you're using Candid Core Framework in your project, we'd love to hear about it!
- **Spread the Word** - Help us improve geospatial metadata by sharing the framework with others

---

We're excited to have you contribute to making geospatial data more usable through Data Candor!
