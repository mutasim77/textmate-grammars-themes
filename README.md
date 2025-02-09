# tm-grammars / tm-themes

[![tm-grammars](https://img.shields.io/npm/v/tm-grammars?label=tm-grammars&labelColor=080f12&color=1fa669)](https://www.npmjs.com/package/tm-grammars)
[![tm-themes](https://img.shields.io/npm/v/tm-themes?label=tm-themes&labelColor=080f12&color=1fa669)](https://www.npmjs.com/package/tm-themes)

Collection of TextMate [grammars](./packages/tm-grammars/) and [themes](./packages/tm-themes/), converted in JSON format and re-distributed as npm packages.

Packages are **automatically updated and published** every day (if there are changes).

Scripts are extracted and modified from [Shiki](https://github.com/shikijs/shiki).

## Contribute

### Add a new grammar

1. Fork this repository
2. Add grammar source and metadata to [`sources-grammars.ts`](./sources-grammars.ts)
3. Add a code sample file `<id>.sample` for your language under [`./samples`](./samples). A sample should include a variety of language syntaxes and succinctly capture the idiosyncrasy of a language. Format requirements:
  - Space for indentation
  - Less than 100 columns if possible
  - Link to source in the last line, for example `# From https://poignant.guide/book/chapter-5.html`
4. Run `pnpm run fetch` to download the grammar and verify it works
5. Send in the PR!

### Add a new theme

1. Fork this repository
2. Add theme source and metadata to [`sources-themes.ts`](./sources-themes.ts)
3. Run `pnpm run fetch` to download the theme and verify it works
4. Send in the PR!

## License

The grammars included in this package are covered by their repositories’ respective licenses, which are permissive (apache-2.0, mit, etc), and made available in [Grammars NOTICE](./packages/tm-grammars/NOTICE) and [Themes NOTICE](./packages/tm-themes/NOTICE).

All other files [MIT](./LICENSE) © Pine Wu & Anthony Fu
