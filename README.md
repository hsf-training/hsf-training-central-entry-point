# A central entry point for all HEP Training content

## The idea

At HSF Training, we have created a [curriculum/training center](hepsoftwarefoundation.org/training/curriculum.html), that links to a series of training modules, most of which we develop ourselves. However, there are clearly more resources out there! But the page is clearly already getting crowded, requiring us to focus on one particular _style_ of training and a very limited scope.

Could we do better though? Probably! If we create a more "dynamic" page with various menus for filtering training resources, we could create a _central entry point_ for every student who wishes to boost their software skills. Students could filter by experiemnt, by technology, by level, or by training paradigm. Different selections of modules could be combined into a whole _series_ of individual curricula that can be pointed out by advisers.

For more information, see the [proposal](https://docs.google.com/document/d/e/2PACX-1vQDpRvrAjRaJFMvjZQ84l_piLimfzsYIwk4NadGNVmd8apgJeUDsXMKKOkwWVleWVTqhTCQM5jKHOb_/pub).

## A fork from learn.astropy.org

This repository is a clone of the repository that hosts the homepage of the Astropy Learn project, https://learn.astropy.org and serves the content from the [astropy-tutorials](https://github.com/astropy/astropy-tutorials) repository. The site itself is built with [Gatsby](https://www.gatsbyjs.com/) and the [Algolia](https://www.algolia.com) search service. Records for the Algolia database are curated and formatted by the [learn-astropy-librarian](https://github.com/astropy/learn-astropy-librarian) app.

Show them your support by leaving a star or back-propagating any improvements/fixes that also apply to them.

## Developer guide

### Initial set up

Create a fork on https://github.com/astropy/learn.

```bash
npm install
```

### Run a development server

You can run a development server that will serve the site and reload as you develop the app:

```bash
npm run develop
```

By default the app is hosted at http://localhost:8000. You can also interact with the GraphQL data layer by browsing

### Build for production

```bash
npm run build
```

Preview the built site by running:

```bash
npm run serve
```

### Linting and autoformatting

This app uses ESLint to lint JavaScript, which in turn runs Prettier to format JavaScript. The configuration is based on [wesbos/eslint-config-wesbos](https://github.com/wesbos/eslint-config-wesbos).

A Git pre-commit hooks runs both ESLint and Prettier and automatically lints and reformats code before every commit. These hooks are run by [husky](https://typicode.github.io/husky/#/) and should already be installed when you ran `npm install`.

To manually lint the code base:

```bash
npm run lint
```

To also fix issues and format the code base:

```bash
npm run lint:fix
```

Ideally your editor will also apply eslint/prettier on save, though these commands are handy as a fallback.

### About the node version

This project is intended to be built with a Node.js version that's encoded in the [`.nvmrc`](./.nvmrc) file. To adopt this Node version, we recommend installing and using the [node version manager](https://github.com/nvm-sh/nvm).

Then you can use the preferred node version by running `nvm` from the project root:

```sh
nvm use
```

### Additional resources for developers

Learn more about Gatsby:

- [Documentation](https://www.gatsbyjs.com/docs/?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter)
- [Tutorials](https://www.gatsbyjs.com/tutorial/?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter)
- [Guides](https://www.gatsbyjs.com/tutorial/?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter)
- [API Reference](https://www.gatsbyjs.com/docs/api-reference/?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter)
- [Plugin Library](https://www.gatsbyjs.com/plugins?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter)
- [Cheat Sheet](https://www.gatsbyjs.com/docs/cheat-sheet/?utm_source=starter&utm_medium=readme&utm_campaign=minimal-starter)

Learn more about Algolia:

- [Documentation](https://www.algolia.com/doc/)
- [React instantsearch](https://www.algolia.com/doc/guides/building-search-ui/what-is-instantsearch/react/)
