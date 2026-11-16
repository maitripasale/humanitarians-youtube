# FACTCHECK — website-load-balancing

General system-design concepts; no statistics are claimed.

| # | Claim (beat) | Verdict |
|---|---|---|
| 1 | One server's capacity is limited by CPU, memory and network; overload slows then crashes it (B01) | TRUE — standard capacity limits |
| 2 | A lone server is a single point of failure (B01) | TRUE |
| 3 | Scaling up (bigger machine) has a ceiling and is costly; scaling out = horizontal scaling (B02) | TRUE |
| 4 | A load balancer sits in front; clients reach it, it forwards to a server in the pool; looks like one site (B03) | TRUE — reverse-proxy / LB model |
| 5 | Round robin rotates; least connections picks the least busy; IP hash pins a client to a server (sticky sessions) (B04) | TRUE — standard algorithms (e.g. NGINX, HAProxy, AWS ELB docs). "Least busy" = fewest active connections |
| 6 | Health checks every few seconds remove failed servers (B05) | TRUE — intervals are configurable, typically seconds (e.g. AWS ALB default 30 s; "every few seconds" is a common setting, not a fixed rule) |
| 7 | Autoscaling adds servers on spikes, removes them after (B05) | TRUE |
| 8 | Multi-region pools; DNS-based / anycast routing to the nearest healthy region (B05) | TRUE |
| 9 | CDN serves images and video from nearby caches (B05) | TRUE |
| 10 | Load balancer must be redundant (pairs or managed service) (B06) | TRUE |
| 11 | The database is often the next bottleneck (B06) | TRUE — common in practice; "often", not always |
