# Koinos Lists

Moderated lists for Koinos.

Inspired by [Uniswap's token lists](https://github.com/Uniswap/token-lists)


## Semantic versioning

Lists include a `version` field, which follows [semantic versioning](https://semver.org/).

List versions must follow the rules:

- Increment major version when elements are removed
- Increment minor version when elements are added
- Increment patch version when elements already on the list have minor details changed (name, symbol, logo URL, decimals, etc..)

Changing a token address or chain ID is considered both a remove and an add, and should be a major version update.

Note that list versioning is used to improve the user experience, but not for security, i.e. list versions are not meant
to provide protection against malicious updates to a list; i.e. the list semver is used as a lossy compression
of the diff of list updates. List updates may still be diffed in the client dApp.