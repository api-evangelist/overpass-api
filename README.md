# Overpass API

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

Read-only OpenStreetMap data API for querying geographic features, nodes, ways, relations, and tags using the Overpass Query Language for complex spatial queries.

**Human URL:** https://overpass-api.de/

**Base URL:** https://overpass-api.de/api

## Description

Overpass API is a read-only API optimized for querying OpenStreetMap data. It supports retrieval of nodes, ways, relations, and areas using the Overpass Query Language (QL) or XML syntax, with output in JSON, XML, CSV, or custom formats. The API is free to use with no authentication required, operated by FOSSGIS as a community service.

## Key Resources

- [Documentation](https://dev.overpass-api.de/overpass-doc/en/)
- [OSM Wiki](https://wiki.openstreetmap.org/wiki/Overpass_API)
- [Query Language Reference](https://wiki.openstreetmap.org/wiki/Overpass_API/Overpass_QL)
- [Overpass Turbo (Interactive)](https://overpass-turbo.eu/)
- [GitHub Repository](https://github.com/drolbr/Overpass-API)
- [API Status](https://overpass-api.de/api/status)

## Primary Endpoint

```
POST/GET https://overpass-api.de/api/interpreter
```

### Example Query (JSON output)

```
[out:json][timeout:25];
node["amenity"="cafe"](48.8,2.3,48.9,2.4);
out body;
```

## Plans

- [Plans](plans/plans.yml)
- [Rate Limits](rate-limits/rate-limits.yml)
- [FinOps](finops/finops.yml)

## License

Overpass API software is licensed under [AGPL-3.0](https://github.com/drolbr/Overpass-API/blob/master/LICENSE). OSM data is available under the [Open Database License (ODbL)](https://www.openstreetmap.org/copyright).
