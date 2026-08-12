# Pimento

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

Pimento is an AI ad-creative platform (Create, Analyze, Benchmark, Brand Kit, Meta Score,
multiformat, Meta Advantage+), surfaced as a portfolio company of Partech. Sector: AI/ML.

## Why this profile is thin

Pimento has **no developer program**. A contract-discovery pass on 2026-08-12 probed every
Pimento host and found:

- `www.pimento.design` and `app.pimento.design` are client-rendered single-page apps whose edge
  answers HTTP **200 with the identical shell** for every path — including `/openapi.json`,
  `/llms.txt` and every `/.well-known/*`. Those 200s are catch-alls, not documents.
- `api.pimento.design`, `docs.pimento.design`, `developer(s).pimento.design`, `status.pimento.design`
  and `blog.pimento.design` do **not resolve**.
- A real, private API does exist: `https://app.pimento.design/api/*` answers
  `401 {"detail":"Unable to authenticate"}`, guarded by Pimento's Auth0 tenant
  `gopimento.eu.auth0.com` with the audience `https://api.gopimento.co` (which itself does not
  resolve in public DNS). It is the web app's own backend — undocumented, unreferenced, and not
  offered to third parties.
- No OpenAPI, AsyncAPI, GraphQL SDL, Postman collection, MCP server, A2A agent card, SDK,
  package, CLI, changelog, status page or public pricing page was found anywhere.

What **is** published and captured here: an Intercom help centre with a real (if near-empty)
`llms.txt`, the Auth0 OIDC discovery document, TLS/DNS posture, and an honest zero for plans and
rate limits. The Intercom `security.txt` served at `help.pimento.design` is **Intercom's own**
(canonical `app.intercom.com`) and is deliberately not credited to Pimento.

Backed by: partech — https://www.pimento.design/
