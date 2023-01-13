# API Specifications

**_Single Source of Truth for Merkez API_**

This is repository to store all Merkez api specifications. This repo is read-only by default except for those who have admin role.

## Visualize and/or Edit API Specification

### Recommended way

If you use VSCode as IDE, you can use [OpenAPI (Swagger) Editor](https://marketplace.visualstudio.com/items?itemName=42Crunch.vscode-openapi) VSCode Extension to visualize and edit the specification

### Another way

You can use [Swagger UI](https://swagger.io/tools/swagger-ui/download/) to visualize and use [Swagger Editor](https://swagger.io/tools/swagger-editor/download/) to edit the specification.

# Linting, and Bundling API Specification

You need to install [Redocly CLI](https://redocly.com/docs/cli/installation/) globally to lint, bundle, and manage the api specification.

## Linting

```bash
redocly lint openapi.yaml
```

Above command will validate the openapi.yaml file against the rules describeb in .redocly.yaml.

_Note: you can ignore warning or error from linting result in .redocly.lint-ignore.yaml_

## Bundling

Combine the multi-file definition into single openapi.yaml file.

```bash
redocly bundle vBeta/openapi.yaml -o openapi_beta.yaml
```
