# Changelog

## 2.3.0

- New **API Endpoints** view in the Explorer: every route in the workspace grouped by class. Filter by URL, path or keyword (same matching as Search Endpoint), click to open the method, copy a request from the inline button. Refreshes after Java files are saved, created or deleted.

## 2.2.0

- New **Feedback** command (Copy Request menu and Command Palette): opens a prefilled bug report or feature request at [hi-mamba/feedback](https://github.com/hi-mamba/feedback).
- A one-time prompt after 20 copies invites a Marketplace review. The counter stays in VS Code's local storage and is never sent.
- Marketplace Q&A enabled.
- License: from 2.2.0 the extension is distributed under a proprietary license — free to use, including for commercial projects. Earlier versions remain under MIT.

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
