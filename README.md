# Action Golang with cache

GitHub Action for setting up Golang via [actions/setup-go](https://github.com/actions/setup-go) coupled with [actions/cache](https://github.com/actions/cache) to cache Golang module and build cache directories.

Designed for use with Linux based runners.

## Usage

```yaml
jobs:
  main:
    name: Use Golang
    runs-on: ubuntu-latest
    steps:
      - name: Setup Golang with cache
        uses: flipgroup/action-golang-with-cache@main
        with:
          version: ~1.17
          cache-key-suffix: key-suffix # optional input argument
```
