# zeroshot-releases

This repository holds the release binaries of the `zeroshot` CLI for macOS and Linux, with `SHA256SUMS`.

Releases are published by zeroshot's CI from tags. No source code lives here.

## Install

Download `zeroshot-<os>-<arch>` and `SHA256SUMS` from
`https://github.com/kool-mn/zeroshot-releases/releases/download/<tag>/`, then verify:

```sh
sha256sum --ignore-missing -c SHA256SUMS
# on a Mac:
shasum -a 256 --ignore-missing -c SHA256SUMS
```

Install and check:

```sh
install -m 0755 zeroshot-<os>-<arch> ~/.local/bin/zeroshot
zeroshot version
```
