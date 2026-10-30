# toil-lab

Two Claude Code agents, a developer and a DevOps engineer, build and run a
small app on a local Kubernetes cluster. They work only through GitHub issues
and pull requests, and a human approves every merge.

| Repo | Contents |
|---|---|
| [agents](https://github.com/toil-lab/agents) | The `dev-agent` and `ops-agent` plugins, their guard hooks, and the `service.yaml` contract |
| [platform](https://github.com/toil-lab/platform) | The cluster, tenancy, GitOps, and the Terraform for this org |
| [checks](https://github.com/toil-lab/checks) | statuspage services that run uptime checks |
| [status](https://github.com/toil-lab/status) | statuspage services that store and show the results |

Each pull request records the human minutes it took, how many times a human
had to step in, and what changed in the agents because of it.
