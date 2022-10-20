# Javascript Example - Non-Snowplow Data

For this example, the input data is a json string which looks like this: 

```json
{
  "name": "Bruce",
  "id": "b47m4n",
  "batmobileCount": 1
}
```

The script filters out any data with a `batmobileCount` less than 1, otherwise it updates the Data's `name` field to "Bruce Wayne", and sets the PartitionKey to the value of `id`:

```js reference
https://github.com/snowplow-incubator/stream-replicator-examples-temp/blob/main/docs/docs/documentation-examples/configuration/transformations/custom-scripts/examples/js-non-snowplow-script-example.js
```

The configuration for this script is:

```hcl reference
https://github.com/snowplow-incubator/stream-replicator-examples-temp/blob/main/docs/docs/documentation-examples/configuration/transformations/custom-scripts/examples/js-non-snowplow-config-example.hcl
```