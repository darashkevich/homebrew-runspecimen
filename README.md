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
`runspecimen-0.2.0rc14.tar.gz` from GitHub Release `v0.2.0-rc.14`:

<https://github.com/darashkevich/runspecimen/releases/download/v0.2.0-rc.14/runspecimen-0.2.0rc14.tar.gz>

sha256 `6ffcfe2fba33dea6b4b8bdf9369f8a05b5d4e286a1e8e01ec46bdbb81cfc4af3`

That release includes Antigravity/Muse adapters and QA fixes on top of opt-in
isolation, policy, and retain. Default backend `none` does not confine the
process. The formula does not enable an OS sandbox. Published `0.2.0rc12`
rejects `isolation` and `policy`.

Upstream project: <https://github.com/darashkevich/runspecimen>  
Product site: <https://runspecimen.darashkevich.com/>  
License: Apache-2.0

## Updating the formula

When a new GitHub Release ships, update `url` and `sha256` in
`Formula/runspecimen.rb` to match the release asset (and keep the in-tree copy
at `packaging/homebrew/runspecimen.rb` in the main repo in sync).
