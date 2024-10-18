# Redocly Bundle Issue Minimal Reproduction

See [Redocly/redocly-cli 1776](https://github.com/Redocly/redocly-cli/issues/1776)

When the buld command below is run:

```
npx @redocly/cli bundle -o ./generated/
```

A single file named generated.yaml in the ./ folder with the content from ./openapi/pet-store.yaml:

```
.
└── generated.yaml
```

Before v1.23.0, it would output one file per spec file to the ./generated/ folder.

```
.
├── generated
    ├── museum.yaml
    └── petstore.yaml
```
