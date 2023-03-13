# Upgrade Version Action

Upgrade the version of the repository in the `package.json`

> This action requires you to upgrade through a script called release. A easy way to do this is a package like [standard-version](https://www.npmjs.com/package/standard-version).

## Usage

```yaml

- name: Upgrade Version
    uses: clockwork-marketing-uk/actions-upgrade-version@1.0.0
    with:
        github-user: ${{ github.actor }}

```


### Release Script

Example using standard version

```json
{
    "scripts": {
        "release": "standard-version",
        "release:first": "npm run release -- --first-release",
    },
}

```
