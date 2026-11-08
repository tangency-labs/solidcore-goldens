# solidcore-goldens

Golden data for [solidcore](https://github.com/tangency-labs/solidcore)'s tests, kept out of the main repository so ordinary checkouts and CI jobs don't download it.

| Folder | What it is | From |
|---|---|---|
| `expected/` | Each golden unit's committed expected output (`crates/goldens/expected` in solidcore) | solidcore `7257e4ca03de5a7f739c54f996d9a5fd42fa4282` |
| `fixtures/` | Input fixtures the goldens and tests read (`fixtures/` in solidcore) | solidcore `7257e4ca03de5a7f739c54f996d9a5fd42fa4282` |

The kernel pins this repository by commit and fetches it only for the jobs and commands that run the goldens. To change a golden, open a pull request here, then bump the pin in the kernel in the same change that needs it.

Licensed under the Apache License 2.0, the same as solidcore (see `LICENSE`).
