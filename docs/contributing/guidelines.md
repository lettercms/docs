---
sidebar_position: 2
---

# Guia de contribución

Para contribuir de manera mas organizada tenemos algunos parametros a seguir para realizar contribuciones de mejor manera y agilizar el proceso, siempre siguiendo el [Código de Conducta](.) de nuestra comunidad.

## Desarrollo

El proyecto completo esta alojado en **[GitHub](https://github.com/lettercms)**. 

Primero que nada, por favor antes de hacer un pull ruequest con una nueva funcionalidad o un cambio grande en el proyecto, crear una nueva incidencia para discutir dichos cambios.



Here's the table of contents:
- [Setup the Project](#setup-the-project)
  - [Commands](#commands)
- [Updating the docs for new release](#updating-the-docs-for-new-release)
  - [Commit Convention](#commit-convention)
  - [Steps to PR](#steps-to-pr)
- [Want to write a blog post or tutorial](#want-to-write-a-blog-post-or-tutorial)
- [Want to help improve the docs?](#want-to-help-improve-the-docs)
- [License](#license)

## Setup the Project


### Commands

**`pnpm`**: installs the dependency packages.

**`pnpm dev`**: starts the local development server.

**`pnpm build`**: builds the docsite for production.

**`pnpm lint`**: runs the nextjs linter which checks for code issues.

**`pnpm avatars:gen`**: regenerates the avatars

**`pnpm members:gen`**: regenerates the members

**`pnpm former-members:gen`**: regenerates the former members

**`pnpm search-meta:gen`**: regenerates the search meta

**`pnpm showcase-data:gen`**: regenerates the showcase data

**`pnpm changelog:gen`**: regenerates the Changelog

**`pnpm cache:clean`**: deletes the `.contentlayer` folder

**`pnpm clean`**: deletes the `pnpm.lock` file and `node_modules`

**`pnpm reinstall`**: reinstalls the dependency packages



### Commit Convention

Before you create a Pull Request, please check whether your commits comply with
the commit conventions used in this repository.

When you create a commit we kindly ask you to follow the convention
`category: message` in your commit message while using one of
the following categories:

- `feat`: all changes that introduce completely new code or new features
- `fix`: changes that fix a bug (ideally you will additionally reference an
  issue if present)
- `refactor`: any code related change that is not a fix nor a feature
- `docs`: changing existing or creating new documentation (i.e. README, docs for
  usage of a lib or cli usage)
- `build`: all changes regarding the build of the software, changes to
  dependencies or the addition of new dependencies
- `ci`: all changes regarding the configuration of continuous integration (i.e.
  github actions, ci system)
- `chore`: all changes to the repository that do not fit into any of the above
  categories

If you are interested in the detailed specification you can visit
https://www.conventionalcommits.org/ or check out the
[Angular Commit Message Guidelines](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#-commit-message-guidelines).

### Steps to PR

1. Fork of the lettercms/sdk repository and clone your fork

2. Create a new branch out of the `main` branch. We follow the convention
   `[type/scope]`. For example `fix/accordion-hook` or `docs/menu-typo`. `type`
   can be either `docs`, `fix`, `feat`, `build`, or any other conventional
   commit type. `scope` is just a short id that describes the scope of work.

3. Make and commit your changes following the
   [commit convention](https://github.com/chakra-ui/chakra-ui-docs/blob/main/CONTRIBUTING.md#commit-convention).
   As you develop, you can run `yarn lint` to make sure everything works as
   expected. Please note that you might have to run `yarn` first in order to
   install all dependencies.


## For maintainers

We use [a custom script](https://github.com/nextauthjs/next-auth/blob/main/scripts/release/index.ts) together with [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0) to automate releases. This makes the maintenance process easier and less error-prone. Please study the "Conventional Commits" site to understand how to write a good commit message.

When accepting Pull Requests, make sure the following:

- Use "Squash and merge"
- Make sure you merge contributor PRs into `main`
- Rewrite the commit message to conform to the `Conventional Commits` style.
  - Using `fix` releases a patch (x.x.1)
  - Using `feat` releases a minor (x.1.x)
  - Using `feat` when `BREAKING CHANGE` is present in the commit message releases a major (1.x.x)
- Optionally link issues the PR will resolve (You can add "close" in front of the issue numbers to close the issues automatically, when the PR is merged. `semantic-release` will also comment back to connected issues and PRs, notifying the users that a feature is added/bug fixed, etc.)

### Skipping a release

If a commit contains `[skip release]` in their message, it will be excluded from the commit analysis and won't participate in the release type determination. This is useful, if the PR being merged should not trigger a new `npm` release.

## License

By contributing your code to the lettercms GitHub repository, you agree to
license your contribution under the Apache-2.0 license.****
