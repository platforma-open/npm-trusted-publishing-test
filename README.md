# npm-trusted-publishing-test

Canary for npm trusted publishing (OIDC) through the shared `github-ci` workflow
(MILAB-7081). The build runs on a self-hosted runner, packs the packages, and a
GitHub-hosted job uploads them to npm with an OIDC token.

The two packages are not meant to be used. `published-from.txt` in each tarball
records the runner where `prepublishOnly` ran.
