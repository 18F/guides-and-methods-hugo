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

## Create new content 

1. Add single files with `hugo new <SECTIONNAME>/<FILENAME>.<FORMAT>`.
1. Add a new guide (aka section) with `hugo new --kind section-bundle <SECTIONNAME>`

## Architectural Decision Records

Check out our ADR directory (just [one so far](https://github.com/18F/guides-and-methods-hugo/pull/3#event-7726496797)) for a history of architectural decisions!

## Contact
Open a GitHub issue and assign to the `@guides-admins` group.
