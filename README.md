# Sana Benefits (sana-benefits)

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
