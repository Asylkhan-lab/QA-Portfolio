# API Testing Notes (Sample)

Target: JSONPlaceholder (public fake API)

## What to check
- Status codes (200/201/400/401/403/404/500)
- Response body schema (required fields, types)
- Headers (Content-Type, caching)
- Pagination/filtering (if exists)
- Error messages format
- Security basics (auth, rate limits) — if applicable

## Example test scenarios
- GET list endpoint returns array
- GET by id returns object and correct id
- Invalid id returns 404
