# Kortix vs Eigent

Both Kortix and Eigent are open source. They are built around different units: Eigent is a Cowork desktop app that runs agents on one person's machine, and Kortix is a platform a whole company runs and governs from one repository.

## The head-to-head

| Dimension | Kortix | Eigent |
| --- | --- | --- |
| What it is | The open-source AI Operating System | An open-source Cowork desktop |
| Where agents run | One isolated cloud computer per session, on its own branch | On your own machine, local-first |
| Unit of ownership | A company: agents, skills, memory and connectors in one git repo | A desktop workspace |
| Governance | Per-resource permissions for people and agents; approval gates; an audit trail | SSO and access control on the Enterprise tier |
| Models | Any provider with your own keys, or the ChatGPT plan you already pay for | Cloud APIs, enterprise gateways, or local inference |
| Finished work | Opens a change request; merge is default-deny for agents | Runs on the desktop |
| Hosting | Kortix Cloud, your VPC, or on-prem; self-host is free | The desktop app; an optional managed cloud |
| License | Open source | Apache 2.0 |

Eigent's rows come from its own repository, [github.com/eigent-ai/eigent](https://github.com/eigent-ai/eigent), checked October 2026: it describes a local-first desktop app built on CAMEL-AI, a multi-agent workforce, and Enterprise features such as SSO and access control. Kortix's rows come from the [Kortix docs](https://kortix.com/docs).

## When Eigent is the right fit

Pick Eigent when one person wants agents working on their own files, on their own machine, with no cloud account. That is exactly what a local-first desktop app is for, and Eigent is explicit that local deployment is its recommended mode.

## When Kortix is the right fit

Pick Kortix when more than one person shares the agents and the work has to be governed. One git repo holds every agent, skill, memory file and connector. Per-resource permissions decide what a person or an agent may touch. Each session is isolated, tool calls can be Allow, Ask or Block, and finished work lands through a change request a person reads as a diff. Self-host it free, run it in your VPC, or use Kortix Cloud.

## The short decision

One person, own machine, no account: Eigent. A team or company that needs shared, governed agents on infrastructure it controls: Kortix.
