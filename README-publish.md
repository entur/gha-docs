# publish

Publish your developer documentation.

## Usage

By following the golden path, with docs in `./docs` and repo name = project name:

```yaml
  publish-docs:
    uses: entur/gha-docs/.github/workflows/publish.yml
    secrets: inherit
```

In case your repository is not named the same as your docs project, or if you do not place docs in `./docs` use this: 

```yaml
  publish-docs:
    uses: entur/gha-docs/.github/workflows/publish.yml
    with:
      project: the-project
      directory: path/to/docs
    secrets: inherit
```

## Inputs

<!-- AUTO-DOC-INPUT:START - Do not remove or modify this section -->

|                            INPUT                            |  TYPE  | REQUIRED |    DEFAULT    | DESCRIPTION |
|-------------------------------------------------------------|--------|----------|---------------|-------------|
| <a name="input_directory"></a>[directory](#input_directory) | string |  false   |   `"docs"`    |             |
|    <a name="input_project"></a>[project](#input_project)    | string |  false   | `"repo_name"` |             |

<!-- AUTO-DOC-INPUT:END -->

## Outputs

<!-- AUTO-DOC-OUTPUT:START - Do not remove or modify this section -->
No outputs.
<!-- AUTO-DOC-OUTPUT:END -->
