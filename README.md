```bash
┌─ damien@homelab ~ ───────────────────────────────────────────────────────┐
│                                                                           │
│ $ cat /etc/sre/profile                                                   │
│ Focus areas:                                                             │
│ • Kubernetes & container orchestration                                   │
│ • Infrastructure as Code (Terraform, Helm, Ansible)                      │
│ • Observability (Prometheus, Grafana, Elasticsearch)                     │
│ • Incident response & SLO management                                     │
│                                                                           │
│ $ tree -L 4 ~/workspace/infra-monorepo/                                  │
│ infra-monorepo/                                                          │
│ ├── terraform/                                                           │
│ │   ├── modules/           # Reusable components                        │
│ │   └── stacks/            # aws, azure, gcp, cloudflare                │
│ ├── kubernetes/                                                          │
│ │   ├── base/              # Base manifests                              │
│ │   └── overlays/          # Kustomize per env/cluster                  │
│ │       ├── prod-aws-us1/                                                │
│ │       ├── prod-az-we1/                                                 │
│ │       ├── prod-gcp-eu1/                                                │
│ │       └── staging-gcp-eu1/                                             │
│ ├── ansible/                                                             │
│ │   ├── playbooks/         # Configuration management                   │
│ │   └── roles/             # Reusable automation                        │
│ └── monitoring/                                                          │
│     ├── dashboards/        # Grafana JSON                                │
│     └── alerts/            # Prometheus rules                            │
│                                                                           │
│ $ echo $PHILOSOPHY                                                        │
│ "Nothing is magic. If you want it done, do it yourself."                 │
│                                                                           │
│ $ uptime                                                                  │
│  up 36 years   |   Systems stable. Coffee adequate.                      │
│                                                                           │
└───────────────────────────────────────────────────────────────────────────┘
```
