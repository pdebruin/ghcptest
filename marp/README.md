# Marp Presentation

This folder contains a Marp presentation for the ghcptest repository.

## What is Marp?

**Marp** (Markdown Presentation Ecosystem) allows you to create beautiful slide decks using Markdown. It's built on:

- **Marpit**: The core framework for slide deck transformation
- **Marp Core**: The engine that powers Marp presentations
- **Marp CLI**: The command-line interface for converting Markdown to slides

## Files

- `slides.md`: The main presentation file in Markdown format
- `theme.css`: Custom theme with Segoe UI font and Microsoft Student Hub colors

## Building Locally

To build the presentation locally, run:

```bash
npx @marp-team/marp-cli@latest marp/slides.md --theme marp/theme.css -o dist/index.html
```

This will generate an HTML presentation in the `dist` folder.

## GitHub Pages Deployment

The presentation is automatically deployed to GitHub Pages when changes are pushed to the `main` branch. The deployment is handled by the `.github/workflows/deploy-marp-slides.yml` workflow.

## Viewing the Presentation

Once deployed, the presentation will be available at:
`https://pdebruin.github.io/ghcptest/`

## Editing the Presentation

Edit the `slides.md` file to modify the presentation. Use Markdown syntax with special Marp directives:

- Start with frontmatter to enable Marp:
  ```markdown
  ---
  marp: true
  theme: default
  paginate: true
  ---
  ```

- Use `---` to separate slides

## Resources

- [Marp Official Documentation](https://marp.app/)
- [Marpit Framework](https://marpit.marp.app/)
- [Marp CLI](https://github.com/marp-team/marp-cli)
- [Example Repository](https://github.com/pelikhan/skillup-github-agentic-workflows)
