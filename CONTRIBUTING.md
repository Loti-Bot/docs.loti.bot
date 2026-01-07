# Contributing

### Commit Guidelines

Create a descriptive branch in your fork before opening a PR on main. Examples:

- `fix-typo`
- `edit-autoresponse`
- `add-new-module-notes`

## Quick Rules

- Headings: reserve `#` for titles, start content at `##`, keep sentence case, add `<Icon>` for command headings, and step down with `###` only.

- Commands: wrap `Syntax` and `Example` plaintext blocks inside one `<CodeGroup>`.
- Components: keep `<Tip>`/`<Info>` to two sentences; use `<CardGroup>/<Card>` for multiple links and `<Tabs>/<Tab>` for comparisons.

- Formatting: leave blank lines between bullets, document options under `### Parameters` with bolded names, and build tables with pipes, hyphens, and bold headers.
- Links: prefer root relative paths (for example, `./variables`)include notable info

## Language translations contributions

- Location & structure:

  - Avoid moving or renaming files unless absolutely necessary.
  - Keep filenames and relative paths identical to the source so links remain consistent.

- Frontmatter:

  - Translate `title` and `description`. Keep `order`, `icon`, and other navigation fields unless a change is required.
  - Ensure `title` and `description` remain concise for navigation.

- Content rules:

  - Preserve code blocks, inline code, placeholders and variables exactly (`{user}`, `%s`, `{count}`, `<tag>`, etc.).
  - use consistent translations for technical terms. When a term is ambiguous, include the original term in parentheses on first mention.
  - Maintain original formatting for `##`/`###` headings and component usage (`<CodeGroup>`, `<Tip>`, `<Card>`, etc.).
  - For pluralization do not remove keys, translate forms according to the original plural structure.
  - Use proper punctuation/spacing for the target language.

- PR guidelines:

  - Branch name: include locale and purpose, e.g., `es-add-guides`.
  - PR title: include language code and scope, e.g., `Add Spanish (es) translations for settings`.
  - In PR description include:
    - Which directories/files were added or updated.
  - If adding partial translations, mark pages as WIP and open separate PRs per major section when possible.

## Snippet for a new doc

````mdx
---
icon: shield
order: 0
title: "Feature Name"
description: "Short summary for navigation."
---

find more info via https://www.mintlify.com/docs/

## <Icon icon="shield" size={32} /> `,command`

<CodeGroup>
    ```plaintext Syntax
    ,command (required) [optional]
    ```

        ```plaintext Example
        ,command #channel message content
        ```

</CodeGroup>

### Description

Explain the command in one or two sentences.

### Parameters

- `(required)`
- `[optional]`
````
