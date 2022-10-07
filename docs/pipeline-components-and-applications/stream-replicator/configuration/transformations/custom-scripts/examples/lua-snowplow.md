# Lua Example - Snowplow Data

For this example, the input data is a valid Snowplow TSV event - so we can enable `snowplow_mode`, which will convert the data to a JSON before passing it to the script as a Lua table.

The script filters out non-web data, based on the `platform` value, otherwise it checks for a `user_id` value, setting a new `uid` field to that value if it's found, or `domain_userid` if not.

It also sets the partitionKey to `app_id`.

```lua reference
https://github.com/snowplow-incubator/stream-replicator-examples-temp/blob/main/docs/docs/documentation-examples/configuration/transformations/custom-scripts/examples/lua-snowplow-script-example.lua
```

The configuration for this script is:

```hcl reference
https://github.com/snowplow-incubator/stream-replicator-examples-temp/blob/main/docs/docs/documentation-examples/configuration/transformations/custom-scripts/examples/lua-non-snowplow-config-example.hcl
```