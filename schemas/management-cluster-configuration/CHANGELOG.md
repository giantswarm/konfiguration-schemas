# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project's packages adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [v1.1.0] - 2026-03-20

### Added

- Added optional additional layers for supporting stages:
  - `default-stages`: located om `default/stages` with support for default config map values
    and app-specific config map and secret templates.
      - secret values are not supported here because of our policy not share decryption keys across installations.
  - customer `stages`: located in `stages` with support for customer-specific config map values and app-specific
    config map and secret templates.
      - secret values are not supported here because of our policy not share decryption keys across installations.

## [v1.0.0] 2025-08-06

### Added

- Added an equivalent description and formalization of the original Giant Swarm management cluster
  configuration structure.

[v1.1.0]: https://github.com/giantswarm/konfiguration-schemas/tree/management-cluster-configuration/v1.1.0/schemas/management-cluster-configuration
[v1.0.0]: https://github.com/giantswarm/konfiguration-schemas/tree/management-cluster-configuration/v1.0.0/schemas/management-cluster-configuration
