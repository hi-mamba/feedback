# Changelog

## 2.1.0

- **Search Endpoint**: paste a URL (or type a path / keywords) to find the controller method that handles it. Enter opens the method; the copy button copies its request as cURL. Path variables, gateway prefixes and `GET /path` queries all match.
- OpenFeign `@FeignClient` interfaces: the client `path` is used, and a literal `url` becomes the base URL.
- Spring 6 HTTP interfaces: `@HttpExchange`, `@GetExchange`, `@PostExchange`, `@PutExchange`, `@PatchExchange`, `@DeleteExchange`.
- Marketplace icon, clearer description and a user-focused README.

## 2.0.4

- Copy directly by default even when sample values need review. New setting `requestCopier.previewOnWarnings` opens Preview automatically for warnings.

## 2.0.3

- Warnings for every selected request are shown above the preview editor, with localized explanations.

## 2.0.2

- Correct JSON-RPC argument binding. Interface available in 14 languages.
