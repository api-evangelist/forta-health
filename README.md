# Forta Health

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Forta Health operates the largest virtual Applied Behavior Analysis (ABA) network in the United States,
delivering autism therapy to children through two models: Virtual ABA over a HIPAA-secure telehealth
platform across 43 states, and In-Home ABA in Dallas, Houston and San Antonio, Texas. Founded in 2021,
Forta pairs Board Certified Behavior Analysts (BCBAs) who design and supervise individualized treatment
plans with Registered Behavior Technicians and trained parents who deliver live sessions, using
proprietary software and machine-learning models to personalize each plan.

> **Not Forta Network.** This profile covers Forta Health (fortahealth.com), a healthcare company. It is
> unrelated to Forta Network (forta.network), a blockchain security project that shares the name.

## API surface

Forta Health publishes **no public developer program** — no developer portal, documentation, API
reference, SDKs, CLI, sandbox, status page or changelog, and no self-serve API signup.

It does operate a private clinical-operations REST API behind its provider application at
`app.fortahealth.com`. That service publishes its OpenAPI 3.1.0 description anonymously at
`https://api.prod.fortahealth.com/openapi.json` (450 operations, 306 paths, 578 schemas, HTTP bearer
auth), which is the machine-readable surface this profile is built from. Every data operation on that
API is correctly authenticated — anonymous requests return `403 Not authenticated`, and only the health
check answers without a token. No patient, staff or other record was retrieved, and none appears in this
repository.

Because the API's resources are protected health information concerning children, and because no
authorized third-party caller exists, **no Agent Skills and no MCP tool manifest were authored** for this
provider. That exclusion is deliberate and is recorded in [`skills/_index.yml`](skills/_index.yml). Full
detail of what was probed, found and withheld is in [`review.yml`](review.yml).

- Company: https://www.fortahealth.com/
- GitHub: https://github.com/fortahealth
- Secondary-market listing: https://www.hiive.com/securities/forta-health-stock
