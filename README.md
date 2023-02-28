# YAML file validation using a remote JSON schema

Validates a YAML file by converting it to JSON and validating it using a JSON schema retrieved from a remote API endpoint.

## Inputs

### `api-endpoint`

**Required** The HTTP API endpoint which returns the JSON schema.

### `yaml-file`

**Required** The name of the YAML file to validate.

## Example usage

```yaml
- name: YAML file validation
  uses: fpesce/nexus-validate-using-remote-schema-action@main
  with:
    api-endpoint: https://json.schemastore.org/github-action.json
    yaml-file: action.yml
```
