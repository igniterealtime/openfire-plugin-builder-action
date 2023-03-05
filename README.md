# Openfire Plugin builder action

GitHub Action to build an Openfire Plugin

Intended to be called by an Ignite Realtime repository, but there might be some use to others too.

## Usage

Assumes the calling repository has access to the secrets.

```yaml
jobs:
  build:
    uses: Fishbowler/openfire-plugin-builder-action/.github/workflows/openfire-plugin-build.yml@main
    secrets:
      IGNITE_REALTIME_MAVEN_USERNAME: ${{ secrets.IGNITE_REALTIME_MAVEN_USERNAME }}
      IGNITE_REALTIME_MAVEN_PASSWORD: ${{ secrets.IGNITE_REALTIME_MAVEN_PASSWORD }}
```
