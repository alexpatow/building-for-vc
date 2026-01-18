# Contributing to Building for VC

Thank you for your interest in contributing to this site! Contributions from the community help make this resource more valuable for everyone building technology at venture capital funds.

## Ways to Contribute

- **Report errors or typos** - Found something wrong? Open an issue or submit a PR
- **Suggest improvements** - Ideas for better explanations, additional examples, or new topics
- **Add examples from your experience** - Real-world examples make the content more valuable
- **Update vendor/tool information** - Technology changes quickly; help keep recommendations current
- **Share dissenting opinions** - Different perspectives strengthen the content

## Before Contributing

1. **Review existing chapters** to understand the book's tone (direct, opinionated, practical)
2. **Check existing issues** to see if your topic is already being discussed
3. **Consider scope** - This book focuses on VC funds specifically, not general startup advice

## Content Guidelines

### Voice and Tone

- **Direct and opinionated**: Take clear positions. "Don't build your own CRM" not "You might want to consider..."
- **Second-person "you"**: Address the reader directly
- **Technical but accessible**: Assume technical competence but explain VC-specific context
- **No buzzwords**: Avoid corporate speak, marketing language, and hype
- **Practical over theoretical**: Focus on what to actually do, with real examples

### Structure Requirements

- **Start with thesis statements**: First sentence should state what the section covers
- **Use "The Bottom Line" summaries**: Many chapters end with practical takeaways
- **Include code examples**: Always add language tags for syntax highlighting
- **Real examples**: Reference specific tools, vendors, and approaches where possible

### What Doesn't Belong

- Generic startup or tech company advice
- Comprehensive coverage of every option (this book makes specific recommendations)
- Future speculation about technology that doesn't exist yet
- Marketing content or vendor pitches

## Technical Setup

### Prerequisites

- [Bun](https://bun.sh/) installed (JavaScript runtime and package manager)
- Git for version control
- Text editor of your choice

### Getting Started

1. **Fork and clone the repository**:

   ```bash
   git clone https://github.com/YOUR-USERNAME/building-for-vc.git
   cd building-for-vc
   ```

2. **Install dependencies**:

   ```bash
   bun install
   ```

3. **Run the local development server**:

   ```bash
   bun run dev
   ```

   This starts Mintlify at `http://localhost:3000`

4. **Check formatting**:

   ```bash
   bun run format:check
   ```

5. **Auto-fix formatting issues**:
   ```bash
   bun run format
   ```

## Making Changes

### Workflow

1. **Create a feature branch**:

   ```bash
   git checkout -b fix-typo-in-data-modeling
   ```

2. **Make your changes**:
   - Edit MDX files in the appropriate directory
   - Follow existing patterns for structure and formatting
   - Add code examples with language tags
   - Keep the direct, opinionated voice

3. **Test locally**:
   - Run `bun run dev` and verify your changes render correctly
   - Check both light and dark modes
   - Verify any links work

4. **Format your code**:

   ```bash
   bun run format
   ```

   Note: Pre-commit git hooks automatically check formatting, so this will be enforced before commits.

5. **Commit your changes**:

   ```bash
   git add .
   git commit -m "Fix typo in data modeling chapter"
   ```

   Write clear, descriptive commit messages. The git hooks will automatically verify formatting.

6. **Push to your fork**:
   ```bash
   git push origin fix-typo-in-data-modeling
   ```

### Commit Message Guidelines

- Use present tense: "Fix typo" not "Fixed typo"
- Be specific: "Update PitchBook pricing in data providers" not "Update content"
- Reference issues when applicable: "Fix #123: Clarify entity resolution approach"

## Pull Request Process

1. **Create a pull request** from your fork to the main repository
2. **Describe your changes clearly**:
   - What problem does this solve?
   - What specific changes did you make?
   - Reference any related issues
3. **Be open to feedback** - Maintainers may suggest revisions
4. **Respond to review comments** - Discussion improves the content
5. **Be patient** - Reviews may take a few days

### What Makes a Good PR

- **Focused scope**: One logical change per PR (fix a typo, add an example, update a section)
- **Clear description**: Explain what changed and why
- **Tested locally**: You've verified the changes render correctly
- **Properly formatted**: `bun run format` has been run
- **Maintains voice**: Changes match the book's direct, practical tone

## File Structure

```
building-for-vc/
├── part-1-understanding-vc/     # Chapters 1-3: VC fundamentals
├── part-2-tech-stack/           # Chapters 4-12: Tools and platforms
├── part-3-technical-foundations/ # Chapters 13-23: Technical deep dives
├── docs.json                    # Navigation and site configuration
├── index.mdx                    # Homepage
├── quickstart.mdx               # Reading guide
└── README.md                    # Project documentation
```

All chapters are written in MDX (Markdown + JSX components) with YAML frontmatter:

```yaml
---
title: "Chapter Title"
description: "Brief description for SEO and navigation"
---
```

## Questions or Issues?

- **Open an issue** for questions, bugs, or feature requests
- **Start a discussion** for broader topics or ideas
- **Reach out directly** to [Alex Patow on LinkedIn](https://www.linkedin.com/in/alexpatow/)

## License

By contributing, you agree that your contributions will be licensed under the same license as the project (see [LICENSE](LICENSE)).

---

Thank you for helping make this resource better for everyone building technology at venture capital funds!
