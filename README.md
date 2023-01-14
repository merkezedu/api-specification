# API Specifications

**_Single Source of Truth for Merkez API_**

[https://merkezedu.github.io/api-specification/](https://merkezedu.github.io/api-specification/)

This is repository to store all Merkez api specifications. This repo is read-only by default except for those who have admin role.

**The actual API specification is `openapi.yaml`**, the other files are needed for API designing purpose.

You can choose API version by selecting the specific branch, branch `main` contains the latest version of the API specification.

## Visualize and/or Edit API Specification

If you use VSCode as IDE, you can use [OpenAPI (Swagger) Editor](https://marketplace.visualstudio.com/items?itemName=42Crunch.vscode-openapi) VSCode Extension to visualize and edit the specification

## Linting, and Bundling API Specification

You need to install [Redocly CLI](https://redocly.com/docs/cli/installation/) globally to lint, bundle, and manage the api specification.

### Linting

```bash
redocly lint openapi.yaml
```

Above command will validate the openapi.yaml file against the rules describeb in .redocly.yaml.

_Note: you can ignore warning or error from linting result in .redocly.lint-ignore.yaml_

### Bundling

Combine the multi-file definition into single openapi.yaml file.

```bash
redocly bundle vBeta/openapi.yaml -o openapi_beta.yaml
```
