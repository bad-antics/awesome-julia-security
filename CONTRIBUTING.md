# Contributing to Awesome Julia Security

Thank you for your interest in contributing to the most comprehensive security resource list for the Julia ecosystem!

## How to Contribute

### Adding a Package

1. Make sure the package is related to security, cryptography, privacy, or related fields
2. The package should be publicly available on GitHub or a similar platform
3. Add your package in alphabetical order within its category
4. Use the following format:

```markdown
- [Package Name](https://github.com/user/package) - Short description ending with a period.
```

### Quality Standards

- Description must start with a capital letter and end with a period
- Description should be concise (one line) and clearly explain what the package does
- Package should have a README with basic documentation
- Package should be installable via `Pkg.add()` or clonable from Git
- No duplicate entries across sections (choose the most relevant category)

### Categories

If your package doesn't fit an existing category, feel free to suggest a new one. Categories should have at least 2 items.

### What We're Looking For

- Julia packages for cryptographic primitives and protocols
- Network security and analysis tools built with Julia
- Binary analysis and reverse engineering tools
- Machine learning models for security applications
- Privacy-preserving computation frameworks
- Security scanning and vulnerability research tools
- Educational resources about security in Julia

### What We Won't Accept

- Packages that are clearly abandoned (no commits in 3+ years with open breaking issues)
- Malicious tools designed solely for unauthorized access
- Packages that violate the Julia community code of conduct
- Marketing-heavy descriptions or promotional content

## Submitting Changes

1. Fork this repository
2. Create a new branch: `git checkout -b add-package-name`
3. Make your changes following the guidelines above
4. Run a spell check on your additions
5. Submit a pull request with a clear description of what you're adding

## Reporting Issues

- If a linked package is broken, archived, or no longer available, open an issue
- If you find incorrect categorization, open a PR with the fix
- If you have suggestions for the list structure, open a discussion

## Code of Conduct

Be respectful and professional in all interactions. This is a security-focused list — ensure all packages are legitimate, well-intentioned, and serve the security research community.
