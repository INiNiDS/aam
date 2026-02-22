Contributing to AAM

First off, thank you for taking the time to contribute! It’s people like you who make AAM a better asset format for everyone.

As a project focused on efficiency and performance, we value high-quality, well-tested, and documented contributions.
📜 Code of Conduct

By participating in this project, you agree to abide by our community standards: stay professional, be respectful, and focus on constructive feedback.
🛠 How Can I Contribute?
1. Reporting Bugs

    Check the Issues to see if the bug has already been reported.

    If not, open a new issue. Include:

        A clear description of the bug.

        Steps to reproduce it.

        Environment details (OS, Compiler/Rust version).

        If possible, an example .aam file that causes the issue.

2. Suggesting Format Changes

Since AAM is a binary format, changes to the specification are sensitive.

    Please start a thread in GitHub Discussions before writing code.

    Explain the problem your change solves and the impact on file size/parsing speed.

3. Improving Documentation

    Our documentation is built with Docusaurus.

    You can fix typos, clarify technical details, or add new guides in the docs/ folder.

🚀 Development Workflow

    Fork the repository.

    Clone your fork: git clone https://github.com/your-username/aam.git

    Create a branch for your feature: git checkout -b feat/my-new-feature

    Make your changes.

        For the docs: Use pnpm install and pnpm start.

        For the parser: Ensure you follow the existing coding style (e.g., cargo fmt for Rust).

    Commit your changes using Conventional Commits:

        feat: add support for texture compression

        fix: resolve buffer overflow in header parser

        docs: update memory layout specification

    Push to your fork and open a Pull Request.

🧪 Testing Criteria

    Any new feature in the parser must include unit tests.

    If you modify the specification, ensure the documentation and implementation remain in sync.

💬 Communication

If you have questions or want to brainstorm, join our [Telegram](t.me/ininids) or start a GitHub Discussion.
