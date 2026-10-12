# Compatibility Notes

## Intended compatibility
The Skill uses plain Markdown instructions and reference files, making it easy to inspect, fork, and adapt. Host platforms differ in skill discovery, metadata parsing, reference loading, and instruction priority. Compatibility is intended, not guaranteed.

## What may vary
- Required metadata fields and folder naming.
- Skill discovery and activation.
- Whether reference files load automatically or must be read explicitly.
- Context limits and instruction retention.
- Tool access, file creation, and confirmation rules.

## Porting checklist
1. Check the host platform's required format and metadata.
2. Keep core behavior in the primary instruction file.
3. Inline relevant reference guidance if reference loading is unsupported.
4. Respect platform tool and confirmation requirements.
5. Run `tests/test-cases.md`.
6. Document platform-specific changes.
