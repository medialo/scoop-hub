# scoop-hub

**H**osted **U**tility **B**ucket, or in other words: another [Scoop](https://scoop.sh) bucket.

A single place to install the command-line tools I build on Windows.

## Getting started

Install [Scoop](https://scoop.sh) if you don't have it yet:

```pwsh
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

Add the bucket:

```pwsh
scoop bucket add hub https://github.com/medialo/scoop-hub
```

Install an app:

```pwsh
scoop install hub/gogws
```

## Apps

| App | Version | Description | Platforms | License | Manifest |
| --- | --- | --- | --- | --- | --- |
| [gogws](https://github.com/medialo/gogws) | [![gogws](https://img.shields.io/scoop/v/gogws?bucket=https://github.com/medialo/scoop-hub&label=)](https://github.com/medialo/gogws/releases/latest) | Manage a folder full of Git repositories as one workspace: status, fetch, pull and clone them all in parallel. | x64, arm64 | [AGPL-3.0](https://github.com/medialo/gogws/blob/master/LICENSE) | [gogws.json](https://github.com/medialo/scoop-hub/blob/master/bucket/gogws.json) |

## Updating

```pwsh
scoop update            # refresh Scoop and every bucket
scoop update gogws      # update one app
scoop update *          # update every installed app
```

## Uninstalling

```pwsh
scoop uninstall gogws
scoop bucket rm hub
```

## Issues

Problems with an app belong in that app's repository. Open an issue here only for problems with the bucket or a manifest itself.
