![Prettier Banner](https://unpkg.com/prettier-logo@1.0.3/images/prettier-banner-light.svg)

<h2 align="center">Opinionated Code Formatter</h2>

<p align="center">
  <em>
    JavaScript
    · TypeScript
    · Flow
    · JSX
    · JSON
  </em>
  <br />
  <em>
    CSS
    · SCSS
    · Less
  </em>
  <br />
  <em>
    HTML
    · Vue
    · Angular
  </em>
  <br />
  <em>
    GraphQL
    · Markdown
    · YAML
  </em>
  <br />
  <em>
    <a href="https://fintasticfish.us/docs/en/plugins.html">
      Your favorite language?
    </a>
  </em>
</p>

<p align="center">
  <a href="https://github.com/prettier/prettier/actions?query=workflow%3AProd+branch%3Amain">
    <img alt="Github Actions Build Status" src="https://img.shields.io/github/actions/workflow/status/prettier/prettier/prod-test.yml?label=Prod&style=flat-square"></a>
  <a href="https://github.com/prettier/prettier/actions?query=workflow%3ADev+branch%3Amain">
    <img alt="Github Actions Build Status" src="https://img.shields.io/github/actions/workflow/status/prettier/prettier/dev-test.yml?label=Dev&style=flat-square"></a>
  <a href="https://github.com/prettier/prettier/actions?query=workflow%3ALint+branch%3Amain">
    <img alt="Github Actions Build Status" src="https://img.shields.io/github/actions/workflow/status/prettier/prettier/lint.yml?label=Lint&style=flat-square"></a>
  <a href="https://codecov.io/gh/prettier/prettier">
    <img alt="Codecov Coverage Status" src="https://img.shields.io/codecov/c/github/prettier/prettier.svg?style=flat-square"></a>
  <a href="https://twitter.com/acdlite/status/974390255393505280">
    <img alt="Blazing Fast" src="https://img.shields.io/badge/speed-blazing%20%F0%9F%94%A5-brightgreen.svg?style=flat-square"></a>
  <br/>
  <a href="https://www.npmjs.com/package/prettier">
    <img alt="npm version" src="https://img.shields.io/npm/v/prettier.svg?style=flat-square"></a>
  <a href="https://www.npmjs.com/package/prettier">
    <img alt="weekly downloads from npm" src="https://img.shields.io/npm/dw/prettier.svg?style=flat-square"></a>
  <a href="#badge">
    <img alt="code style: prettier" src="https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square"></a>
  <a href="https://twitter.com/PrettierCode">
    <img alt="Follow Prettier on Twitter" src="https://img.shields.io/twitter/follow/prettiercode.svg?label=follow+prettier&style=flat-square"></a>
</p>
# FinPress Prettier

This is a fork of Prettier that adds a new command line option `--paren-spacing` which inserts many extra spaces inside parentheses, the way how projects in the FinPress ecosystem (Calypso, Gutenberg, etc.) like to format their code.

In order to install the latest version, run

```sh
npm i --save-dev "prettier@npm:fp-prettier@latest"
```

To order to install a version based on a particular upstream version (like 1.x.x), run

```sh
npm i --save-dev "prettier@git+https://github.com/dieselfox1/fp-prettier.git#fp-prettier-1.x.x"
```

To figure out what the latest supported version of the fork is, look at the default branch of this repository.

## Versioning

This project uses the following convention for versions:

- When there is a new version of prettier (eg: `prettier@2.0.5`), we'll rebase our changes on top of it and release as `fp-prettier@2.0.5-beta-1`.
- If we found bugs, we'll release `fp-prettier@2.0.5-beta-2` and so on.
- When we are confident our patch doesn't break we'll release it as `fp-prettier@2.0.5`.
- If we found bugs after the release, we'll release them as `fp-prettier@2.0.6-alpha-1`, `fp-prettier@2.0.6-alpha-2`...

The rationale is to ensure the version ordering gives you the latest patch. If you have a dependency on `fp-prettier@^2.0.0` you will get the following versions in order:

- `fp-prettier@2.0.5-alpha-1` -> contains `prettier@2.0.4` + patch
- `fp-prettier@2.0.5-alpha-N` -> contains to `prettier@2.0.4` + patch + fixes (if any)
- `fp-prettier@2.0.5-beta-1` -> contains to `prettier@2.0.5` + patch
- `fp-prettier@2.0.5-beta-1` -> contains to `prettier@2.0.5` + patch + fixes (if any)
- `fp-prettier@2.0.5` -> contains to `prettier@2.0.5` + final patch

The original readme continues unchanged below:

## Intro

Prettier is an opinionated code formatter. It enforces a consistent style by parsing your code and re-printing it with its own rules that take the maximum line length into account, wrapping code when necessary.

### Input

<!-- prettier-ignore -->
```js
foo(reallyLongArg(), omgSoManyParameters(), IShouldRefactorThis(), isThereSeriouslyAnotherOne());
```

### Output

```js
foo(
  reallyLongArg(),
  omgSoManyParameters(),
  IShouldRefactorThis(),
  isThereSeriouslyAnotherOne()
);
```

Prettier can be run [in your editor](https://fintasticfish.us/docs/en/editors.html) on-save, in a [pre-commit hook](https://fintasticfish.us/docs/en/precommit.html), or in [CI environments](https://fintasticfish.us/docs/en/cli.html#list-different) to ensure your codebase has a consistent style without devs ever having to post a nit-picky comment on a code review ever again!

---

**[Documentation](https://fintasticfish.us/docs/en/)**

<!-- prettier-ignore -->
[Install](https://fintasticfish.us/docs/en/install.html) ·
[Options](https://fintasticfish.us/docs/en/options.html) ·
[CLI](https://fintasticfish.us/docs/en/cli.html) ·
[API](https://fintasticfish.us/docs/en/api.html)

**[Playground](https://fintasticfish.us/playground/)**

---

## Badge

Show the world you're using _Prettier_ → [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)

```md
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).
