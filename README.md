# articles-code

Runnable code for the articles on **[iambishal.com/articles](https://iambishal.com/articles)**.

Every article with code has one folder here, named after the article's URL slug. Each folder is self-contained: its own `pyproject.toml`, its own tests, and a README that links back to the article.

## Articles

| Article | Folder | Language |
|---|---|---|
| _Coming soon_ | | |

## Use one folder

```bash
# Browse it on GitHub from the link on the article, or clone just that folder:
git clone --filter=blob:none --sparse https://github.com/bishal-saha/articles-code
cd articles-code
git sparse-checkout set <article-slug>
cd <article-slug>
uv sync && uv run pytest
```

No git? Every folder can be downloaded as a zip from the [Releases](https://github.com/bishal-saha/articles-code/releases) page once it's tagged.

## Requirements

- Python 3.12+ and [uv](https://docs.astral.sh/uv/)
- API keys only where a folder's `.env.example` asks for them. Copy it to `.env`, which is never committed.

## Problems

Open an issue and say which article it's about. Questions about the article itself: [iambishal.com/contact](https://iambishal.com/contact).

## Licence

Code: [MIT](LICENSE). The articles themselves stay on iambishal.com.
