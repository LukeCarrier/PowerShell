# Build PowerShell as a Flatpak

This guide will walk you through building PowerShell on Linux as a Flatpak.
For now we'll only cover building on Ubuntu, but additional distributions will follow.

## Environment

These instructions are written assuming the Ubuntu 18.04 LTS, since that's the distro Luke uses.
The build module works on a best-effort basis for other distributions.

### Git Setup

Using Git requires it to be set up correctly;
refer to the [Working with the PowerShell Repository](../git/README.md),
[README](../../README.md), and [Contributing Guidelines](../../.github/CONTRIBUTING.md).

**This guide assumes that you have recursively cloned the PowerShell repository and `cd`ed into it.**

### Toolchain Setup

Install `flatpak-builder`:

```
$ sudo apt install flatpak-builder
```

## Build using Flatpak

```
$ flatpak-builder flatpak-build com.microsoft.PowerShellCore.json
```
