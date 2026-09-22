# Homebrew tap for RunSpecimen

Installs the published RunSpecimen CLI from GitHub Release assets
(not from `main`).

## Install

```bash
brew tap darashkevich/runspecimen
brew install runspecimen
```

Or in one step:

```bash
brew install darashkevich/runspecimen/runspecimen
```

## What this installs

`Formula/runspecimen.rb` pins the published sdist
`runspecimen-0.2.0rc13.tar.gz` from GitHub Release `v0.2.0-rc.13`:

<https://github.com/darashkevich/runspecimen/releases/download/v0.2.0-rc.13/runspecimen-0.2.0rc13.tar.gz>

sha256 `0a807d65e73adfc2af2c8e5679706ed7c4d881ffefdc36e9222507cf5168f5c5`

That release includes opt-in isolation, policy, and retain. Default backend
`none` does not confine the process. The formula does not enable an OS sandbox.
Published `0.2.0rc12` rejects `isolation` and `policy`.

Upstream project: <https://github.com/darashkevich/runspecimen>  
Product site: <https://runspecimen.darashkevich.com/>  
License: Apache-2.0

## Updating the formula

When a new GitHub Release ships, update `url` and `sha256` in
`Formula/runspecimen.rb` to match the release asset (and keep the in-tree copy
at `packaging/homebrew/runspecimen.rb` in the main repo in sync).
