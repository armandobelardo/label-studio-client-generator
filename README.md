# label-studio-client-generator

## Development

### Generate docs

```
fern generate --docs
```

#### Generate docs locally
```
fern docs dev
```

## Add custom docs

Go to `fern/openapi/overrides.yaml` and modify fields keeping the structure as in `fern/openapi/openapi.yaml`. For example

```
paths:
  /api/projects/:
    post:
      summary: List of Projects
```
-->
```
paths:
  /api/projects/:
    post:
      summary: A new title to be replaced
    get:
      description: and another update in description `/get` endpoint.
```
