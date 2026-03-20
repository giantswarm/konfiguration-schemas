# Management Cluster Configuration

This schema is an equivalent description and formalization of the original Giant Swarm management cluster
configuration structure - `konfigure generate` - in the Generalized Configuration System.

On top of the original structure, optional additional layers got added for supporting stages:

- `default-stages`: located om `default/stages` with support for default config map values
  and app-specific config map and secret templates.
  - secret values are not supported here because of our policy not share decryption keys across installations.
- customer `stages`: located in `stages` with support for customer-specific config map values and app-specific
  config map and secret templates. 
  - secret values are not supported here because of our policy not share decryption keys across installations.
