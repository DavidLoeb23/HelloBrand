# Hello Brand — repository guide

## Repository relationship

This repo (`DavidLoeb23/HelloBrand`) is the **Claude Design / visual design and approval source**.
Production implementation lives in `HelloBrandGroup/hello-brand-dxp` (Next.js/React).

**Flow: DESIGN → APPROVAL → PRODUCTION PORT → QA → DEPLOY**

- `site/*.dc.html` here is approved design source, not deployable code. It must be
  deliberately translated into production React/Next.js components in `hello-brand-dxp` —
  never copied in or treated as directly shippable.
- Do not merge or consolidate the two repositories.
- `DavidLoeb23/HelloBrand` stays under this owner during active design build; a follow-up
  action is recorded to transfer it to `HelloBrandGroup` once the design work is stable.

## Positioning — canonical hierarchy (decided 30 Aug 2026, supersedes prior framing)

- **Hello Brand** — customer relationship, strategy, commercial proposition and execution partner.
- **Hello Brand OS** — Hello Brand-owned orchestration, planning, intelligence and measurement layer.
- **Brand Box** — Hello Brand connected venue/media technology.
- **Social Wiiv** — a specialist execution technology/provider used where appropriate.
- **Twenty** — CRM/relationship infrastructure (internal; not a public product proposition).
- **Other providers** — replaceable specialist execution/measurement technologies.

The provider architecture stays replaceable — no provider is structurally synonymous with
Hello Brand OS. Social Wiiv may be credited on capabilities it actually provides.
**"Powered by Social Wiiv" is not the Hello Brand OS identity and is not a public
destination or site-wide framing.**

Do not alter historical/earlier source documents just because positioning has since evolved.

## Public information architecture

Home → Hello Brand OS → Media + Venues → Brand Box → Measurement + Intelligence → Work → About → Contact.

Connected capabilities may surface within these pages and get promoted to dedicated pages
later when business need justifies it.

## Canonical operating model (preserve everywhere)

- **BRANDS AT PLAY. DATA AT WORK.**
- **PLAN → BOOK → DEPLOY → ACTIVATE → ENGAGE → MEASURE → OPTIMISE**
- Campaign-detail journey: **OBJECTIVE → AUDIENCE → BUDGET → PLAN → MEDIA → VENUES →
  ASSETS → DEPLOYMENT → ACTIVATION → ENGAGEMENT → MEASUREMENT → INSIGHT → OPTIMISATION**
- Measurement provenance: **ESTIMATED → MODELLED → MEASURED → VERIFIED**

## Design authority

Approved Home v2 (`site/Hello Brand OS Home v2.dc.html`) is the current public-site visual
reference. Existing Hello Brand brand assets remain brand authority. The `_ds/modernist...`
token bundle (`site/_ds/modernist-*/styles.css`) plus this file are the **binding source of
truth** for tokens, layout conventions and positioning in this repo — not the UI/UX Pro Max
skill's own dataset.

**UI/UX Pro Max is UX/layout/pattern reasoning only** — a QA/quality-control layer (contrast,
touch targets, focus states, responsive/interaction checks), never a master brand system or
authority to redesign. Never run its `--design-system`/`--persist` flow in this repo — that
generates and writes a new MASTER.md with its own colours/type/spacing, which would compete
with the binding source above. If one of its checks conflicts with the approved tokens or
identity, flag the conflict and ask rather than silently overriding either side.

The earlier "Hello Brand OS 2.0" (Chakra Petch / Plus Jakarta Sans / signal-mark) proposal is
**superseded — exploratory only. Do not implement it.**

Note: `docs/01-design-system.md` and `app/globals.css` (Next.js App Router conventions) do not
exist in this repo — that naming belongs to `hello-brand-dxp`, which this repo's sessions
cannot access. Do not create those paths here to satisfy a request that names them; flag the
mismatch instead.
