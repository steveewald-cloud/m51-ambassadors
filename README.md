# m51-evangelists

**GLORi Evangelist Program** landing page — recruiting for the Marketing51 field
sales force.

## Nomenclature (this is a legal boundary, not a style choice)

**Evangelists are paid GLORi sales reps. Ambassadors are referral customers.**

| | **Evangelists** (this page) | **Ambassadors** |
|---|---|---|
| Who | Paid GLORi field reps | An existing GLORi **customer** |
| Does | Prospects, shares the vision, closes new business | Refers peers *after* becoming a happy customer |
| Paid | Cash commission + residual | Account credit or a Bless — **never cash to a person** |
| Relationship | Disclosed agent of GLORi | Advocate / customer |

The referral program was renamed "GLORi Evangelists" → "GLORi Ambassadors" in the
Ambassadors v1.1 spec, reserving "Evangelists" for the field sales force. This repo
previously used "Ambassador" for the commissioned rep, which inverted the two — see
`OD-Q` in `Glori-Holdings/glori-giving-engine` → `docs/decisions/open-decisions.md`.

The separation matters because "value to the account, never cash to the individual"
is the Ambassadors program's structural anti-kickback defense. A page that blurs
the words undercuts that defense at exactly the moment it would be examined.

**Canonical specs:** `GLORi-Evangelists-FieldSalesForce-v1.0.html` and
`GLORi-Ambassadors-Architecture-v1.1.html`, both in
`Glori-Holdings/glori-giving-engine` → `docs/specs/`.

## Deploy

Static page served by nginx via `Dockerfile`; auto-deploys to Fly on push to `main`
(`.github/workflows/fly-deploy.yml`, needs the `FLY_API_TOKEN` secret).
