# 2. Make menus dynamic

Date: 2022-11-02

## Status

Accepted

## Context

"Right now, the guides all have different ways to implement the side nav." Some use front matter, some use a data.yml file, some define in config.yml.

## Decision

Make menus and page lists dynamic, not hard-coded. Build templates that templates that automatically detect new pages and sections. Top-down approach (template functions), not bottom-up (content front matter).

## Consequences

Adding new content to navigation menus and page lists becomes easier. Reduces number of places a user has to update page and section titles. Facilitates future content management system, since we don't have to add fields that accept more key/value pairs.
