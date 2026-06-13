# Overpass API

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
