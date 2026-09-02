# BrandWell fork modifications

This repository is based on Warmbly and remains subject to the Apache License 2.0 in `LICENSE`.

BrandWell-specific modifications add a private signed service adapter for isolated tenant bootstrap, approved mailbox-cap enforcement, and managed SMTP/IMAP mailbox onboarding. The customer-facing BrandWell product does not use the Warmbly name or dashboard as its own brand surface.

The initial BrandWell adapter work is isolated primarily under:

- `internal/app/brandwell/`
- `internal/api/handler/brandwell.go`
- `internal/repository/pg_brandwell.go`
- `internal/models/brandwell.go`
- `internal/infrastructure/db/migrations/000122_brandwell_service_adapter.*.sql`
- `internal/infrastructure/db/migrations/000123_brandwell_portal_launch.*.sql`
- `docs/content/docs/development/brandwell-service-adapter.mdx`

Existing Warmbly files changed to register or support the adapter are visible in version control history.
