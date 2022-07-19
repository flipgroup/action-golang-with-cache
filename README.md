# Action Golang with cache

GitHub Action for setting up Golang via [actions/setup-go](https://github.com/actions/setup-go) coupled with [actions/cache](https://github.com/actions/cache) to cache Golang module and build cache directories.

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
          version-file: go.mod
          # alternatively, use `version` input
          #version: ~1.18
          cache-key-suffix: key-suffix # optional input argument
```
