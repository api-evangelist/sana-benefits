# Sana Benefits (sana-benefits)

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

Sana Benefits is an Austin, Texas health benefits company founded in 2017 that sells level-funded and self-funded small-group health plans to small and midsize employers in the United States, bundling medical, dental and vision coverage with Sana Care, its in-house virtual-first primary care and care navigation service. Sana distributes almost entirely through licensed benefits brokers, underwrites and administers the plan itself with stop-loss insurance included, and prices provider claims off a reference-based percentage of the Medicare fee schedule.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/sana-benefits/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/sana-benefits/refs/heads/main/apis.yml)

## Tags

- Insurance
- United States
- Health Insurance
- Employee Benefits
- Benefits Administration
- Small Business
- Level-Funded Plans
- Insurtech
- Broker
- Virtual Primary Care

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

None. Sana Benefits publishes no public, self-serve API.

Probed on 2026-07-25: `developer.sanabenefits.com`, `developers.sanabenefits.com`, `docs.sanabenefits.com` and `api.sanabenefits.com` do not resolve, and `/developers`, `/api`, `/developer`, `/partners` and `/integrations` on `www.sanabenefits.com` all return HTTP 404. The 67-URL page sitemap contains no developer, API or integrations page.

The only machine-readable surface is `secure.sanabenefits.com`, the authenticated member / employer / broker application. It serves a JSON shell (`bundleName: "LoginApp"`) and answers `HTTP 401 {"error":{"message":"Login required","code":"login_required"}}` on `/openapi.json`, `/swagger.json` and `/api/v1/openapi.json` — an internal application API behind a session login wall, not a developer product. No OpenAPI, Swagger, AsyncAPI, GraphQL SDL, `.proto`, or Postman artifact is published, so this repo has no `openapi/` directory. There is no GitHub organization.

**ACORD posture: no ACORD reference found.** A word-boundary scan for ACORD, AL3, ACORD XML, NGDS, IVANS, agency download, Applied Epic, Vertafore and AMS360 across the homepage, brokers, partners, employers, FAQ and provider pages returned zero matches. Sana is a health-benefits carrier rather than a P&C carrier, so ACORD is not its native standard — but the health equivalents are equally absent: no X12 834 enrollment, X12 837/835 claims, EDI, SFTP, HRIS/payroll, or SSO integration is described publicly.

**Quote / bind / issue / FNOL:** none exposed programmatically. Quoting is a web form and a broker promise of "rates in 48 hours"; binding runs through the assigned broker; enrollment and issuance happen inside the login-walled employer dashboard; claims are administered by Sana with no FNOL API.

## Links

- [Website](https://www.sanabenefits.com/)
- [Who We Are](https://www.sanabenefits.com/who-we-are/)
- [Plans](https://www.sanabenefits.com/plans/)
- [For Brokers](https://www.sanabenefits.com/brokers/)
- [For Employers](https://www.sanabenefits.com/employers/)
- [Sana Partners](https://www.sanabenefits.com/sana-partners/)
- [Blog](https://www.sanabenefits.com/blog/)
- [Press](https://www.sanabenefits.com/press/)
- [Help Center](https://help.sanabenefits.com/hc/en-us)
- [Sign In](https://secure.sanabenefits.com/)
- [LinkedIn](https://www.linkedin.com/company/sana-benefits/)

## Review

See [review.yml](review.yml) for the full API Evangelist reviewer finding, including every probed URL with its HTTP status.
