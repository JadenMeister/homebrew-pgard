# homebrew-pgard

Homebrew tap for [PGARD](https://github.com/JadenMeister/pgard), a local security scanner for projects you own or are authorized to scan.

```sh
brew tap jadenmeister/pgard
brew trust --formula jadenmeister/pgard/pgard
brew install pgard
```

Recent Homebrew versions load formulae from third-party taps only after you trust them; `--formula` trusts this one formula, not the whole tap.

If `brew link` reports that `bin/pgard` already exists, an npm global install is in the way: run `npm uninstall -g pgard`, then `brew link pgard`.

The formula installs the npm package `pgard` and depends on Homebrew's `node`. It is updated with `packaging/homebrew/update-formula.sh` in the main repository, which checks the npm tarball's provenance before writing the checksum.
