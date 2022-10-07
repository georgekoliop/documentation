# Custom Lua Script Configuration

This section details how to configure the transformation, once a script is written. You can find a guide to creating the script itself in [the create a script section](./create-a-script.md).

You can also find some complete example use cases in [the examples section](./examples/).

The Custom Lua Script transformation uses the [gopher-lua](https://pkg.go.dev/github.com/yuin/gopher-lua) embedded Lua engine to run scripts upon the data.

You can find a guide to writing the scripts themselves - and how the script interfaces with the application - [in the create a script page](./create-a-script.md).

If a script errors or times out, a [transformation failre](/docs/pipeline-components-and-applications/stream-replicator/concepts/failure-model.md) occurs.

Scripts are provided to the configuration as base-64 encoded strings - you can base-64 encode a script with `cat script.js | base64`.


Here is an example of a minimal configuration for the custom Lua script transformation:

```hcl reference
https://github.com/snowplow-incubator/stream-replicator-examples-temp/blob/main/docs/docs/documentation-examples/configuration/transformations/custom-scripts/js-configuration-minimal-example.hcl
```

Here is an example of every configuration option:

```hcl reference
https://github.com/snowplow-incubator/stream-replicator-examples-temp/blob/main/docs/docs/documentation-examples/configuration/transformations/custom-scripts/js-configuration-full-example.hcl
```
