# 06 · Publish

**Purpose:** Send finished posts from `05-output/` to third-party tools and platforms.
**Integrations:** one subfolder per service, e.g. `buffer/`, `linkedin/`, `instagram/`

## Rules
- Read API tokens from environment variables (e.g. `BUFFER_ACCESS_TOKEN`), never from files in this repo.
- Add UTMs to links: `utm_source=<channel>&utm_medium=social&utm_campaign=<post-slug>`.
- Log each publish (service, post, update ID, scheduled time, status) to `publish-log.md`.
