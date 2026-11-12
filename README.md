# Ask AI for MkDocs (free AI chatbot for your docs)

A Material for MkDocs site with an **Ask AI** button next to search. Readers ask in their own words, and the answer is written from your docs, with links to the sections it used. One line in `mkdocs.yml`: no plugin, no crawler, no server.

**Live demo:** https://fengyiqicoder.github.io/mkdocs-ai-chatbot/ (Tally is a made-up product.)

## Add it to your MkDocs site

1. Get a free key at [onetagai.com](https://onetagai.com) (1,000,000 tokens one time, no credit card).
2. Add this to `mkdocs.yml` (or add the line to the `extra_javascript` list you already have):

```yaml
extra_javascript:
  - https://onetagai.com/ask-docs.js?key=YOUR_ONETAG_KEY
```

3. `mkdocs serve` to try it, then deploy as usual (`mkdocs gh-deploy` works).

The script reads the search index MkDocs already builds (`search/search_index.json`), so keep the `search` plugin on. On Material for MkDocs the button sits in the header next to search; on the built-in `mkdocs` and `readthedocs` themes it floats in the corner. Options (label, position, colour, language) are query parameters: see the [guide](https://onetagai.com/guides/mkdocs).

## Run this demo

```sh
pip install mkdocs-material
mkdocs serve
```

## License

MIT
