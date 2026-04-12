# Contributing to Aegis RWA

Thank you for your interest in contributing to the Aegis RWA Protocol! We are building institutional-grade infrastructure on Stellar, and community contributions are vital to our success.

The following is a set of guidelines for contributing to the Aegis RWA organization and its repositories.

##  Getting Help

If you need help, have a question, or want to discuss an architectural change before coding, please:
1. Review our [SUPPORT.md](SUPPORT.md) file.
2. Join the [Stellar Developer Discord](https://discord.gg/stellardev) and tag the Aegis team.

## Branching Strategy

We use a structured branching model. Please name your branches using the following conventions:

* `feat/your-feature-name`: For new features or significant additions.
* `fix/issue-description`: For bug fixes.
* `chore/maintenance-task`: For dependency updates, documentation changes, or internal refactoring.
* `test/what-you-are-testing`: For adding missing tests or CI improvements.

## Pull Request Formatting

To ensure a smooth review process, please adhere to the following standards when submitting a Pull Request (PR):

1.  **Atomic Commits:** Keep your commits focused on a single logical change.
2.  **Descriptive Titles:** Use conventional commit formatting for your PR title (e.g., `feat(contracts): implement batch whitelisting`).
3.  **Link Issues:** Reference the issue your PR resolves in the description (e.g., `Closes #42`).
4.  **Tests:** If you are modifying Rust contracts or the TS SDK, you **must** include accompanying unit tests. PRs without tests will not be merged.
5.  **CI Checks:** Ensure all GitHub Actions (linting, tests, build) pass before requesting a review.

## Code Review Process

All submissions, including those from core team members, require review.
* We aim to review all PRs within 48-72 hours.
* Maintainers may ask for architectural changes or additional tests. Please respond to feedback promptly.
* Once approved by at least one core maintainer, your PR will be squash-merged into the `main` branch.

Thank you for helping us build the future of Real-World Assets on Stellar!