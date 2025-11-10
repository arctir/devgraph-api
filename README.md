# Devgraph API Specification

OpenAPI specification for the Devgraph API.

## Version

Current API version: `1.0.0-beta.1`

## Specification

- **User API**: `v1/spec.yaml` - Main Devgraph API for developers

## Usage

### View in Swagger UI

```bash
docker run -p 8080:8080 -e SWAGGER_JSON=/specs/v1/spec.yaml -v $(pwd)/v1:/specs swaggerapi/swagger-ui
```

### Generate Client Libraries

```bash
# Using OpenAPI Generator
openapi-generator generate -i v1/spec.yaml -g python -o ./devgraph-python-client
openapi-generator generate -i v1/spec.yaml -g typescript-fetch -o ./devgraph-typescript-client
```

## Versioning

This repository is automatically updated when the API specification changes in the main devgraph repository.

- **API Version**: Semantic versioning (see `API_VERSION` file)
- **Git Tags**: Each API version is tagged (e.g., `v1.0.0`, `v1.1.0`)

## Links

- [Main Repository](https://github.com/arctir/devgraph)
- [API Documentation](https://docs.devgraph.ai/api)
- [API Versioning Guide](https://github.com/arctir/devgraph/blob/main/docs/API_VERSIONING.md)

---

Last updated: $(date -u '+%Y-%m-%d %H:%M:%S UTC')
API Version: 1.0.0-beta.1
Commit: 15d7277e593ae9d856c9930c946ddb66dd4c4716
