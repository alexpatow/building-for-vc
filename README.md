<p align="center">
  <img src="logo/dark.svg" alt="Building for VC" width="300">
</p>

# Building for Venture Capital

A comprehensive guide to building technology for venture capital funds, covering everything from understanding VC fundamentals to implementing production infrastructure.

## About This Guide

This guide is for engineers, data people, and technical operators building technology at venture capital funds. It covers:

- **Part 1: Understanding VC** - How VC funds work, fund structures, and common mistakes when starting at a fund
- **Part 2: The VC Tech Stack** - Research platforms, sourcing tools, CRM, fund operations, portfolio support, fundraising, and external presence
- **Part 3: Technical Foundations** - Technology stack selection, data providers, modeling, entity resolution, data quality, warehousing, knowledge graphs, integrations, security, and emerging trends
- **Resources** - Tools, templates, and references to help you build

Based on real experience building VC infrastructure at [Inflection](https://inflection.fund) and [EQT](https://eqtgroup.com).

## Local Development

This site is built with [Mintlify](https://mintlify.com). To preview changes locally:

```bash
bunx mint dev
```

This will start a local development server at `http://localhost:3000`.

## Structure

```
building-for-vc/
├── docs.json                        # Navigation and theme configuration
├── guide/                           # Main guide content
│   ├── index.mdx                    # Homepage
│   ├── quickstart.mdx               # Reading guide
│   ├── part-1-understanding-vc/
│   ├── part-2-tech-stack/
│   └── part-3-technical-foundations/
└── resources/                       # Tools, templates, and references
    └── index.mdx
```

## Content Format

All chapters are written in MDX (Markdown + JSX components) with YAML frontmatter:

```yaml
---
title: "Chapter Title"
description: "Brief description for SEO and navigation"
---
```

## Publishing Changes

This site uses Mintlify's GitHub integration. Changes pushed to the main branch are automatically deployed to production.

## Contributing

If you find errors, have suggestions, or want to contribute additional content, please open an issue or pull request.

For detailed contribution guidelines, see [CONTRIBUTING.md](CONTRIBUTING.md). Feel free to reach out on [LinkedIn](https://www.linkedin.com/in/alexpatow/) or via email at [ap@ınflection.fund](mailto:ap@inflection.fund).

### Code Quality and Formatting

This project uses [Prettier](https://prettier.io/) to maintain consistent formatting across all MDX and JSON files.

**Before committing changes**, check that your files are formatted correctly:

```bash
bun run format:check
```

If there are formatting issues, auto-fix them with:

```bash
bun run format
```

**Git hooks**: This repository uses pre-commit hooks to automatically check formatting before commits. If formatting is incorrect, the commit will be blocked. Run `bun run format` to fix issues, then commit again.

## License

See [LICENSE](LICENSE) for details.

## Resources

- [Mintlify Documentation](https://mintlify.com/docs)
- [MDX Documentation](https://mdxjs.com/)
