# lxorb's Scoop bucket

[![Tests](https://github.com/lxorb/scoop-bucket/actions/workflows/ci.yml/badge.svg)](https://github.com/lxorb/scoop-bucket/actions/workflows/ci.yml) [![Excavator](https://github.com/lxorb/scoop-bucket/actions/workflows/excavator.yml/badge.svg)](https://github.com/lxorb/scoop-bucket/actions/workflows/excavator.yml)

A bucket for [Scoop](https://scoop.sh), the Windows command-line installer.

## Install

```pwsh
scoop bucket add lxorb https://github.com/lxorb/scoop-bucket
scoop install lxorb/nib
```

## Manifests

| App | Description |
| --- | --- |
| [nib](bucket/nib.json) | [Nib](https://nibeditor.com) - a simple, lightweight markdown editor offering all the features you could ever need. Supports x64 and ARM64. |

Manifests are kept up to date automatically by
[Excavator](https://github.com/lxorb/scoop-bucket/actions/workflows/excavator.yml),
which checks upstream releases every four hours, and by the release pipeline of
each app.

## Notes

`nib` is installed portably: Nib's themes and note history live in
`%APPDATA%\ch.emilvinu.nib`, which the manifest junctions into Scoop's persist
directory, so both survive an update or an uninstall.

## Contributing

Manifests follow the Scoop [Contributing
Guide](https://github.com/ScoopInstaller/.github/blob/main/.github/CONTRIBUTING.md)
and the [App Manifests](https://github.com/ScoopInstaller/Scoop/wiki/App-Manifests)
wiki page. Issues and pull requests are welcome.
