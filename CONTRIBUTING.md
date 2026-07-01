# Contributing to Virtual Universe

Thank you for your interest in contributing to the Virtual Universe project! This document provides guidelines and instructions for contributing.

## 🌟 Ways to Contribute

- **Documentation**: Improve specs, add examples, clarify concepts
- **Code Examples**: Add integration samples for different platforms
- **Issue Reporting**: Identify problems or suggest enhancements
- **Pull Requests**: Submit concrete improvements
- **Community Support**: Help other users in Discord and GitHub Discussions

## 🐛 Reporting Issues

Before creating an issue, please:
1. Check if the issue already exists
2. Use the issue templates provided
3. Include as much detail as possible

### Issue Template

```markdown
**Description**
A clear description of the issue or suggestion.

**Steps to Reproduce** (if applicable)
1. Step one
2. Step two
3. ...

**Expected Behavior**
What you expected to happen.

**Actual Behavior**
What actually happened.

**Environment**
- OS: [e.g., Windows 11, macOS 14]
- Node.js version: [e.g., 18.17.0]
- Related tools/versions

**Additional Context**
Any other relevant information, screenshots, or logs.
```

## 🔧 Development Setup

```bash
# Fork and clone the repository
git clone https://github.com/YOUR_USERNAME/virtual-universe.git
cd virtual-universe

# Create a branch for your changes
git checkout -b feature/your-feature-name
```

## 📝 Pull Request Process

1. **Create a Branch**
   ```bash
   git checkout -b feature/amazing-idea
   ```

2. **Make Your Changes**
   - Follow existing code style
   - Add documentation for new features
   - Test your changes thoroughly

3. **Commit Your Changes**
   ```bash
   git add .
   git commit -m "Add: brief description of your changes"
   ```
   
   Use conventional commit prefixes:
   - `Add:` - New features
   - `Fix:` - Bug fixes
   - `Docs:` - Documentation changes
   - `Refactor:` - Code refactoring
   - `Test:` - Adding tests
   - `Chore:` - Maintenance tasks

4. **Push and Create PR**
   ```bash
   git push origin feature/amazing-idea
   ```
   Then open a Pull Request on GitHub.

5. **PR Requirements**
   - Clear description of changes
   - Reference to related issues (if any)
   - Tests passing (if applicable)
   - Documentation updated (if applicable)

## 📚 Documentation Standards

- Use clear, concise language
- Include code examples where helpful
- Update the README.md if adding new features
- Add JSDoc comments to JavaScript functions

### Example Code Documentation

```javascript
/**
 * Get EACO token balance for a wallet
 * @param {string} walletAddress - Solana wallet public key
 * @returns {Promise<number>} Token balance
 */
async function getEacoBalance(walletAddress) {
  // Implementation
}
```

## 🎯 Code Style Guidelines

### JavaScript/TypeScript
- Use `const` and `let` (avoid `var`)
- Use async/await over callbacks
- Add semicolons
- 2-space indentation

### Markdown
- Use proper heading hierarchy
- Include table of contents for long documents
- Use fenced code blocks with language identifiers

## ✅ Code of Conduct

- Be respectful and inclusive
- Welcome newcomers
- Focus on constructive feedback
- Help maintain a positive community

## 🤝 Review Process

All contributions will be reviewed by maintainers. We aim to:
- Review PRs within 7 days
- Provide constructive feedback
- Merge approved changes promptly

## 📧 Contact

- **Discord**: [Join our community](https://discord.gg/HWsweV6fFy)
- **GitHub Issues**: For bug reports and feature requests
- **GitHub Discussions**: For general questions and ideas

---

Thank you for helping make Virtual Universe better! 🚀
