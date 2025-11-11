# Devgraph API Specification

OpenAPI specification for the Devgraph API.

## Version

Current API version: `1.0.0-beta.4`

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

- [API Documentation](https://docs.devgraph.ai/api)

## License

Apache 2.0 - See [LICENSE](LICENSE) file for details.

---

Last updated: 2025-11-11 02:14:01 UTC
API Version: 1.0.0-beta.4
Commit: 2f8f9871752f993abb91e7a8cfaf824d753d4185
