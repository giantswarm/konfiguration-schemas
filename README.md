# Giant Swarm Konfiguration Schema

This repository contains Giant Swarm Konfiguration Schemas for the Generalized Configuration System of [konfigure](https://github.com/giantswarm/konfigure). 

## Working with this repository

This section details how to store schemas in this repository.

### Adding new schemas

All schemas should be stored under the [schemas](schemas) directory under another folder that is named after the
name of the contained schema, for example `schemas/my-schema`.

That directory should contain a file called `schema.yaml`, that contains the raw schema.

That directory should also contain a `README.md` file at least to explain the schema and its use case.

### Tagging schemas

Please tag updates to the schemas manually on the `main` tree in the following format: `my-schema/v1.2.3`, where:

- the first half is the name of the directory under [schemas](schemas)
- a separator of a single `/` character
- the second half is the version, that is always prefixed with `v` followed by a [semantic version](https://semver.org/)

for example:

```shell
git tag my-schema/v1.2.3
git push --tags
```
