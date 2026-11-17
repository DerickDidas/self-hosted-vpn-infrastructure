# Self-Hosted VPN Infrastructure & Protocol Experimentation



## Overview

An independently managed project in which I provisioned a Linux VPS, deployed several VPN and proxy technologies, and troubleshot connectivity from smartphones, Windows computers and other client devices. It began while I was living in China, with the aim of running personally managed VPN connectivity for my own devices and a small number of other users.

## What I did

- Provisioned a KVM VPS running Ubuntu and administered it remotely over SSH (PuTTY).
- Deployed WireGuard first, then configured clients and tested on phones and Windows computers.
- Investigated why the original VPS IP became unreliable for the intended connections, and moved to a replacement IP. The exact cause was **not** established.
- Researched alternative approaches and protocols (VMess, VLESS), including technical discussions on Chinese-language forums.
- Deployed and tested OpenVPN, Hiddify Manager and 3X-UI, using Docker for several of the deployments.
- Ran informal connection, speed and latency checks across devices.

In my own testing, **Hiddify Manager gave the most successful connectivity results**. This is a personal observation from one environment, not a claim that it is better in general.

## Environment (historical)

| Component | Details |
|---|---|
| Provider | RackNerd |
| Virtualization | KVM |
| Location | New York, USA |
| OS | Ubuntu 20.04 (64-bit); historical, not a current recommendation |
| Resources | 1 CPU core, 1 GB RAM, one IPv4 address |
| Tooling | Docker, PuTTY / SSH |
| Period | March 17, 2024 to March 16, 2025 |

## Technologies explored

| Technology | Role in the project |
|---|---|
| WireGuard | First implementation; deployed, configured and tested on client devices |
| OpenVPN | Alternative; the free option I evaluated had limitations |
| Hiddify Manager | Deployed and tested; most successful in my testing |
| 3X-UI | Deployed and tested as a management panel |
| VMess / VLESS | Researched and experimented with as alternative protocols |
| Docker | Used for several deployments |

## Limitations and honesty notes

- No original configs, logs, screenshots or numerical benchmarks survive, so this repo contains **no measured latency, throughput, uptime, CPU or memory figures**.
- The cause of the original IP problem is unconfirmed. I describe it as an observed connectivity/accessibility problem.
- This was an experiment, not a production-grade service, and I make no claims about censorship circumvention.
- Any example added later will be labelled as illustrative or independently recreated.

## Documentation

- [Infrastructure](docs/infrastructure.md)
- [Deployment journey](docs/deployment-journey.md)
- [Technology comparison](docs/technology-comparison.md)
- [Troubleshooting and lessons](docs/troubleshooting.md)
- [Architecture diagram](diagrams/architecture.md)

## Skills demonstrated

Linux/Ubuntu administration, VPS provisioning, SSH, Docker-based deployment, VPN/proxy deployment, connectivity troubleshooting, protocol research, multi-device testing.
