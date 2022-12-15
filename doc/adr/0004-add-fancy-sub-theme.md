# 4. Add fancy sub-theme

Date: 2022-12-08

## Status

Proposed

## Context

<!-- The issue motivating this decision, and any context that influences or constrains the decision. -->

Some guides have a distinct design? How can we allow the flexibility of a different look and feel while still maintaining the best practices established in this repository? Are there components we can reuse?

## Decision

<!-- The change that we're proposing or have agreed to implement. -->
Use Hugo section layouts.

Fancy, being a loose IA label.

The fancy sub-theme includes
card-like style for single pages.
background color option called page_color. Defaults to the USWDS bg-primary-light color.
custom front matter fields. resources is an array of markdown text. considerations is paragraph text.
HTML templates for the custom front matter fields. We need to apply special CSS classes around these areas to hide them in the print version. Which is probably why the original pages included HTML in Markdown. No more! Now we have a custom template.
Other changes
Removed type: card from content pages, since we didn't have this layout.
Changed type: landing to layout: landing, allowing us to still sort by landing pages in the homepage nav and top drop down nav.
Now when type: fancy is applied to a page, it will use one of the fancy templates (single.html and list.html)
We can cascade type: fancy to all pages within a section by including it in the section _index.html front matter. See section5/_index.md.

## Consequences

What becomes easier or more difficult to do and any risks introduced by the change that will need to be mitigated.
