# tomato-reader — build runner

This repository exists only to run a build. It holds no source code.

The source lives in a private repository, and the unsigned IPA that comes out
of a build is published as a release asset **there**, not here — GitHub
artifacts inherit the repository's visibility, so an artifact uploaded to a
public repository is downloadable by anyone. Publishing to the private
repository is what keeps the product out of public reach.

## Where the IPA goes

Releases of the private repository, under the `latest` tag. Each build
replaces the asset, so there is only ever one IPA to download: the newest.

## Running a build

The workflow runs on every push here, and can be started by hand from the
Actions tab.
