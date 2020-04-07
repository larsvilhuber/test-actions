# test-actions

This is a test implementation of combining [Github Actions](https://github.com/features/actions) with [Github Pages](https://pages.github.com/) (i.e, Jekyll).

## Part 1

The first part uses Pandoc to convert a Markdown file into PDF. This is handled by the [.github/workflows/main.yml](https://github.com/larsvilhuber/test-actions/.github/workflows/main.yml) file, parameterizing various Github Actions (`docker`, `git push`). 

This is pushed back to the repository proper (could be a separate branch, such as `gh-pages`), but with a `[noactions]` tag so it does not get processed. 

A more sophisticated workflow would push all to-be-published files into the `gh-pages` branch instead.

## Part 2

Just configure the publication of your repo through Github Pages, in the [settings](settings/). Voilà.

## Result

See [README.pdf](docs/README.pdf).
