# Welcome to the Techdocs for the Catalog

This is a sample techdoc.   The content was pulled from the TAP Workshop.

Publishing Techdocs is a two step process.

1. Generate the Techdocs.
2. Publish the Techdocs.


```
npx @techdocs/cli generate --source-dir catalog --output-dir ./site
```

make sure you have the AWS creds for the target bucket before publishing.

```
npx @techdocs/cli publish --publisher-type awsS3 --storage-name jellin-tanzu-techdocs --entity default/component/dotnet-todos-api --directory ./site
```

The entity is always `default/<entity type>/<name of entity>

Typically entity types are:

* Component
* System
* Resource
* Location
* Api

