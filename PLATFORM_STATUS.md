# Niilox platform — progress overview

**Last updated:** June 2026  
**Production API:** `https://api.niilox.com` · **Portal:** [www.niilox.com](https://www.niilox.com)

High-level status for integrators. Internal runbooks, migration lists, and deployment details are not published here — contact **dev@niilox.com** for partner onboarding.

---

## At a glance

| Layer | Status | Notes |
|-------|--------|-------|
| **Go API** | **Production** | Multi-tenant, native auth |
| **Postgres** | **Production** | Primary + replica |
| **Niilox livestream (broadcast SFU)** | **Production** | Drift tenant |
| **Peer / P2P signaling** | **Production** | GeoGig + Rodent tenants |
| **Developer portal** | **Production** | Keys, billing, SMS, docs at www.niilox.com |
| **SMS + phone numbers** | **Production** | Per-tenant send/bulk, sender config, inventory — [SMS.md](./SMS.md) |
| **`@niilox/sdk`** | **v0.1 beta** | [npm](https://www.npmjs.com/package/@niilox/sdk) — `npm install @niilox/sdk` |

---

## Products on Niilox

| Tenant | Product | Capabilities |
|--------|---------|--------------|
| `drift` | Drift | Niilox livestream, chat, gifts, VIP |
| `geogig` | GeoGig | Gigs, safety, P2P video |
| `rodent` | Rodent | Peer sessions, bookings, drop-off |
| `rabbaly` | Rabbaly | Creator storefront |
| *yours* | Your app | Provision via the portal |

---

## SDK (`@niilox/sdk` v0.1)

TypeScript client with modules for auth, rooms, seats, gifts, payments, gigs, peer, DMs, **SMS**, **numbers**, platform, and more.

**Install:** `npm install @niilox/sdk` · Python: `pip install niilox` — [npm](https://www.npmjs.com/package/@niilox/sdk) · [PyPI](https://pypi.org/project/niilox/)

Sensitive flows (capped events, worker safety, paywall handling) are documented in the private integration guide.

---

## What's next (public roadmap)

- Integration test suite
- Full GeoGig SDK migration
- Niilox KYC and USSD (announcing soon)

For detailed engineering backlog or ops status, contact **dev@niilox.com**.
