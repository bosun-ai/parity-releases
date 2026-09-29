# Parity releases

Release binaries of [Parity](https://bosun.ai), the language for proving that a migrated system behaves like the legacy one. This repository holds release assets only; the source is private.

## Install

Linux x86_64, glibc 2.35 or newer, `curl` or `wget`, and `tar` with xz support:

```sh
curl --proto '=https' --tlsv1.2 -LsSf https://github.com/bosun-ai/parity-releases/releases/latest/download/parity-cli-installer.sh | env PARITY_CLI_NO_MODIFY_PATH=1 sh
```

This installs `parity` into `~/.local/bin`. To install into a fixed directory without touching shell profiles, set `PARITY_CLI_UNMANAGED_INSTALL=/usr/local/bin`.

The installer verifies the archive's sha256; every release also carries `sha256.sum`.

## Versions

- The **latest release** is the supported stable version. It only moves after the release passes a smoke test in Bosun's universal executor image, and maintainers can move it back to an earlier release.
- To pin a version, use `https://github.com/bosun-ai/parity-releases/releases/download/vX.Y.Z/parity-cli-installer.sh`.

Get started with `parity learn`.
