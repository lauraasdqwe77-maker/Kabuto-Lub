# Kabuto-Lub V1.0 · Local-first Commercial Prototype

Mobile-first, three-language navigation, static multi-file prototype for insect breeders. No build tools required.

## Run

Upload `index.html`, `styles.css`, and `app.js` to the **root** of the same GitHub Pages repository and commit. Existing GitHub Pages configuration can continue serving `index.html`. Files must keep their names. Open the Pages URL and refresh.

## Data and migration

Existing V0.2/V0.3 localStorage key `kabuto_insects` is read and preserved. V1.0 additional records use `kabuto_v1_business`. Export a JSON backup **before** upgrading. The Settings page can import V0.2-style `{insects:[...]}` backups and V1.0 backups. Import **replaces** local data, it does not merge. Photos are stored in browser localStorage and are compressed on new uploads; browser quota can still be exceeded.

## Working now

- Insect CRUD, image upload, event timelines
- Parent/offspring navigation when matching codes exist
- Breeding batches, sales records, basic statistics
- Breeder-reported printable pedigree records (not third-party verified)
- Scenario calculator and offline listing template generator
- Chinese/Japanese/English navigation and core UI labels (some forms remain Chinese)
- JSON import/export

## NOT yet implemented

- Accounts, cloud sync, cross-device collaboration, tenant isolation
- Live AI, payments, marketplace APIs, publicly verifiable certificates
- Full localization and production-grade audit/testing

Do **not** offer this prototype to paying customers as a production SaaS. A production backend needs authenticated user accounts, per-tenant authorization, secure media storage, migrations, logging, monitoring, and billing.
