# public-dist

The public distribution of nx2androidX's build artifacts.

Nothing is built here. This repository carries the **release artifacts** of the
product's private build repositories, so that a player - or a CI job - can
fetch them without a token.

## What is here

| release | what it is |
|---|---|
| [memory-embed v2026.11.25](releases/tag/v2026.11.25) | the static embedding model of the local search (`memory_search.py`): `embed.bin` (int8, 40,168 rows x 128 dims), `vocab.txt`, `meta.json` |

The model was trained on the **public corpus only** (the upstream's pull
requests, the knowledge documents and the closed issues of the two
repositories). No player's own case file is in it.

The training code and the corpus live in a private repository
([zFitness/nx2-memory](https://github.com/zFitness/nx2-memory)); this
repository carries the artifact alone.
