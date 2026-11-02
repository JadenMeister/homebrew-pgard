# homebrew-pgard

Homebrew tap for [PGARD](https://github.com/JadenMeister/pgard), a local security scanner for projects you own or are authorized to scan.

```sh
brew tap jadenmeister/pgard
brew install pgard
```

Or in one line: `brew install jadenmeister/pgard/pgard`.

The formula installs the npm package `pgard` and depends on Homebrew's `node`. It is updated with `packaging/homebrew/update-formula.sh` in the main repository, which checks the npm tarball's provenance before writing the checksum.
