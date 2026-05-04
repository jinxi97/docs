# Funky docs

Source for the Funky documentation site at [docs.funky.dev](https://docs.funky.dev).

Built on [Mintlify](https://mintlify.com).

## Local development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint):

```bash
npm i -g mint
```

> Requires Node.js LTS (22). Mintlify does not support Node 25+.

From the repo root (where `docs.json` lives):

```bash
mint dev
```

Preview at `http://localhost:3000`.

## Publishing

Pushes to `main` deploy automatically via the Mintlify GitHub app. No manual step.

## Checking links

```bash
mint broken-links
```

## Troubleshooting

- **Dev server won't start**: run `mint update` to upgrade the CLI.
- **404 on a page**: confirm the path is registered in `docs.json` under `navigation.groups[].pages`.
