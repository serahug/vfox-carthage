# vfox-carthage

A [vfox](https://github.com/version-fox/vfox) plugin for [Carthage](https://github.com/Carthage/Carthage) - a simple, decentralized dependency manager for Cocoa.

## Requirements

- macOS only (Carthage is a Cocoa dependency manager)
- `pkgutil` and `cpio` (included in macOS)

## Installation

```bash
mise use vfox:mise-plugins/vfox-carthage@latest
```

Or add to your `mise.toml`:

```toml
[tools]
"vfox:mise-plugins/vfox-carthage" = "latest"
```

## Usage

```bash
# Check version
carthage version

# Update dependencies
carthage update
```

## How it works

This plugin extracts the carthage binary from the official `.pkg` installer releases using `pkgutil` and `cpio`.

## License

MIT
