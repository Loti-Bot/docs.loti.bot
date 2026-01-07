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
- Links: prefer relative paths (for example, `./variables`) and name the command plus notable flags or other relevant info.

## Starter Snippet

````mdx
---
icon: shield
order: 0
title: "Feature Name"
description: "Short summary for navigation."
---

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
