# guides-and-methods-hugo
18F Guides and Methods using Hugo site engine

This is an experimental repository by the 18F Guides and Methods team.

## Features

* It's on [cloud.gov Pages](https://pages.cloud.gov/sites/1253/builds) 
* Flexible layout templates
* Section specific themes
* Page bundle archetypes
* Improved performance
* Sample governance workflow
* Sample content management workflow
* Multilingual support

## Getting Started (developers)

Please follow the instructions for [Installing Hugo locally](https://gohugo.io/getting-started/usage/).

Anyone that would like to help Dockerize this setup, please contact Claire Annan (@cannandev).

1. Clone `https://github.com/18F/guides-and-methods-hugo.git`
1. `cd` into new directory.
1. Start the built-in live server via `hugo server`.
1. Visit default URL: localhost:1313

### Create new content 

1. Add single files with `hugo new <SECTIONNAME>/<FILENAME>.<FORMAT>`.
1. Add a new guide (aka section) with `hugo new --kind section-bundle <SECTIONNAME>`

## Getting Started (content managers)

In this GitHub repository, find content organized by Section under `content/en`, or use the GitHub search feature to find the file. All content files end in .md for Markdown. To edit a page, 

1. click on the edit pencil.
2. Make content changes. The content supports plain text and [Commonmark](https://commonmark.org/help/) flavored Markdown.
3. Attach files by dragging and dropping, selecting or pasting them.
4. Save your changes by clicking the Commit changes button. This will create a new branch for this commit to start a pull request.
5. The `guides-admins` group (hey, that's us!) is set as the default reviewers.
6. Preview your changes using the cloud.gov Pages preview link.

Keep watching this repo for Content Management System tests. Let us know if you'd like to participate!

## Accessibility

Hopefully you already have pa11y-ci running globally! Hugo generates a default sitemap for each language out of the box. Let pa11y-ci check all the URLs in the sitemap with the following command:

```
pa11y-ci -s http://localhost:1313/en/sitemap.xml --sitemap-find "//localhost:1313" --sitemap-replace "http://localhost:1313/" 
```

## Architectural Decision Records

Check out our ADR directory (just [one so far](https://github.com/18F/guides-and-methods-hugo/pull/3#event-7726496797)) for a history of architectural decisions!

## Contact
Open a GitHub issue and assign to the `@guides-admins` group.
