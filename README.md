# Nous Docs

Source for [docs.opennous.cloud](https://docs.opennous.cloud), the public documentation for **Nous**, the context graph for GTM agents.

Published via [Mintlify](https://mintlify.com). Pushes to `main` deploy automatically.

## Editing

- Content lives under `getting-started/`, `installation/`, `providers/`, `mcp/`, `public-api/`, `webhooks/`, `developer-app/`, `cli/`, and `api-reference/`.
- `docs.json` controls navigation, branding, theme, and navbar/footer links.
- OpenAPI spec at `openapi.json` powers the auto-generated reference pages.

## Preview locally

```bash
npx mint dev
```

Local preview runs at http://localhost:3000.

## Related repos

- Product: https://github.com/NousC/opennous
- Marketing site: https://github.com/NousC/opennous-site (deployed at [opennous.cloud](https://opennous.cloud))

## License

Docs content: see [LICENSE](./LICENSE). Product code is AGPL v3.
