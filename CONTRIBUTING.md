# Contributing to PHP Forge

Thank you for your interest in contributing. Please read this guide before submitting issues or pull requests.

By participating in this project, you agree to abide by the [Code of Conduct](CODE_OF_CONDUCT.md).

## Development Environment

**Requirements:**

- PHP 8.3 or higher.
- [Composer](https://getcomposer.org/) 2.x.

**Setup:**

```bash
git clone https://github.com/php-forge/<repository>.git
cd <repository>
composer install
composer run
```

## Coding Standards

All PHP code must follow these standards:

- **PER 3.0 + PSR-12** coding style.
- `declare(strict_types=1)` in every PHP file.
- Strong typing: use type declarations for parameters, return types, and properties.
- Use [php-forge/coding-standard](https://github.com/php-forge/coding-standard) for automated style checks.

## Testing

- All tests use **PHPUnit 12+**.
- Target **100% code coverage** for new code.
- Run the quality/test scripts defined in the target repository's `composer.json` before submitting a pull request
  (for example, `test`, `static`, `ecs`, `rector`, or `check-dependencies`):

```bash
composer run
```

## Pull Request Process

1. Fork the repository and create a feature branch from `main`.
2. Make your changes in small, focused commits.
3. Use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) for commit messages.
4. One logical change per pull request.
5. Ensure all tests pass and coding standards are met.
6. Open a pull request against `main` with a clear description of the change.

## Security Vulnerabilities

Do not open public issues for security vulnerabilities. See [SECURITY.md](SECURITY.md) for reporting instructions.
