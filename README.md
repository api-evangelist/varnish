# Varnish Cache (varnish)
Varnish Cache is a high-performance HTTP accelerator and reverse proxy designed for content-heavy dynamic websites and APIs. It sits in front of web servers and caches HTTP responses to serve repeated requests without hitting the backend, dramatically reducing load and latency. Varnish is configured via VCL (Varnish Configuration Language), a domain-specific language for request/response policy, and managed through a CLI interface (varnishadm) and a set of command-line tools for logging, statistics, and monitoring.

**URL:** [https://varnish-cache.org/](https://varnish-cache.org/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Caching, Caching Proxy, Content Delivery, HTTP Accelerator, Open Source, Proxy, Reverse Proxy

## Timestamps

- **Created:** 2026-03-27
- **Modified:** 2026-05-03

## APIs

### Varnish Cache CLI API
The Varnish Cache CLI management interface provides programmatic control over a running Varnish instance. It is accessible via varnishadm or TCP socket and supports configuration management (VCL load/use/discard), backend health control, cache ban/invalidation, parameter tuning, and process management. Commands can return JSON output with the -j flag.

**Human URL:** [https://varnish-cache.org/docs/trunk/reference/varnish-cli.html](https://varnish-cache.org/docs/trunk/reference/varnish-cli.html)

#### Tags:

 - Cache Management, Caching, CLI, Configuration, Reverse Proxy

#### Properties

- [Documentation](https://varnish-cache.org/docs/trunk/reference/varnish-cli.html)
- [GettingStarted](https://varnish-cache.org/docs/trunk/users-guide/run_cli.html)
- [APIReference](https://varnish-cache.org/docs/trunk/reference/varnishadm.html)

### Varnish Logging Tools
Varnish ships with a suite of log-analysis tools that read from the Varnish Shared Log (VSL). Tools include varnishlog (raw log streaming), varnishncsa (NCSA/Apache log format), varnishstat (live counters), varnishtop (real-time activity display), and varnishhist (response time histogram).

**Human URL:** [https://varnish-cache.org/docs/trunk/reference/](https://varnish-cache.org/docs/trunk/reference/)

#### Tags:

 - Logging, Monitoring, Observability, Statistics

#### Properties

- [Documentation](https://varnish-cache.org/docs/trunk/reference/varnishlog.html)
- [APIReference](https://varnish-cache.org/docs/trunk/reference/varnishstat.html)

### Varnish Modules (VMODs)
VMODs are extensions written for Varnish Cache that extend VCL capabilities. Bundled modules include blob (binary data handling), cookie (HTTP cookie parsing), directors (load balancing strategies), h2 (HTTP/2 control), proxy (PROXY protocol support), purge (cache purging), std (standard utility functions), and unix (Unix socket support). Additional community VMODs are available for headers, digest, auth, and more.

**Human URL:** [https://varnish-cache.org/docs/trunk/reference/vmod.html](https://varnish-cache.org/docs/trunk/reference/vmod.html)

#### Tags:

 - Extensions, Modules, Plugins, VMODs

#### Properties

- [Documentation](https://varnish-cache.org/docs/trunk/reference/vmod.html)
- [GitHub Repository](https://github.com/varnishcache/varnish-cache)

## Common Properties

- [Website](https://varnish-cache.org/)
- [Documentation](https://varnish-cache.org/docs/)
- [GitHub Organization](https://github.com/varnishcache)
- [GitHub Repository](https://github.com/varnishcache/varnish-cache)
- [ReleaseNotes](https://varnish-cache.org/docs/trunk/whatsNew/)
- [Blog](https://info.varnish-software.com/blog)
- [Forum](https://discourse.varnish-cache.org/)
- [StackOverflow](https://stackoverflow.com/questions/tagged/varnish)

## Features

| Name | Description |
|------|-------------|
| HTTP Caching | Caches HTTP responses to reduce backend load and improve response times for repeated requests. |
| VCL Configuration Language | Domain-specific language for defining request/response handling policies with full programmability. |
| CLI Management Interface | TCP-based management interface for runtime configuration, VCL deployment, and cache control. |
| Backend Health Probes | Configurable health checks for backends with automatic failover to healthy backends. |
| Cache Invalidation (Bans) | Flexible cache invalidation via ban expressions matching any request/response attribute. |
| JSON Output | CLI commands support -j flag for structured JSON output, enabling programmatic management. |
| VMOD Extension System | Loadable modules (VMODs) extend VCL with cookie parsing, load balancing, digest, auth, and more. |
| HTTP/2 Support | Native HTTP/2 support via the h2 VMOD for modern protocol acceleration. |
| Shared Memory Log (VSL) | High-speed shared memory logging with rich request/response attributes for analysis tools. |
| Multi-threaded Architecture | Worker thread pool for high-throughput concurrent request handling with configurable threading. |

## Use Cases

| Name | Description |
|------|-------------|
| API Gateway Caching | Cache REST API responses at the edge to reduce database and application server load. |
| CDN Origin Shield | Act as origin shield between CDN edge nodes and web/application servers. |
| Static Asset Acceleration | Cache and serve static assets (images, JS, CSS) with long TTLs. |
| A/B Testing | Use VCL to route traffic fractions to different backends for controlled experiments. |
| DDoS Mitigation | Absorb traffic spikes and rate-limit abusive clients via VCL policies. |
| Authentication Offloading | Offload token validation and session checks to VCL logic at the cache layer. |
| Request Routing | Route requests to different backend pools based on URL patterns, headers, or cookies. |

## Integrations

| Name | Description |
|------|-------------|
| Nginx | Common deployment pairing with Nginx as backend web server behind Varnish. |
| Apache HTTP Server | Classic deployment with Apache as origin server behind Varnish Cache. |
| Kubernetes | Deployable as a sidecar or DaemonSet in Kubernetes clusters for service-level caching. |
| Prometheus | Varnish statistics exportable via varnish_exporter for Prometheus scraping. |
| Grafana | Community dashboards available for Varnish Cache statistics via Prometheus/Grafana. |
| Drupal | Deep integration with Drupal Cache Tags for efficient purging of cached pages. |
| WordPress | VCL configurations and plugins available for WordPress caching integration. |
| Fastly | Fastly CDN is built on Varnish Cache; Fastly VCL is a fork of Varnish VCL. |

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
