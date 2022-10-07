# spEnrichedFilter Configuration

`spEnrichedFilter`: Filters messages based on a regex match against an atomic field.

This transformation is for use on base-level atomic fields, rather than fields from contexts, or custom events - which can be achieved with `spEnrichedFilterContext` and `spEnrichedFilterUnstructEvent`.

This example filters out all data whose `platform` value does not match either `web` or `mobile`.

Minimal configuration:

```hcl reference
https://github.com/snowplow-incubator/stream-replicator-examples-temp/blob/main/docs/docs/documentation-examples/configuration/transformations/snowplow-builtin/spEnrichedFilter-minimal-example.hcl
```

Every configuration option:

```hcl reference
https://github.com/snowplow-incubator/stream-replicator-examples-temp/blob/main/docs/docs/documentation-examples/configuration/transformations/snowplow-builtin/spEnrichedFilter-full-example.hcl
```