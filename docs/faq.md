# Open source Eigent alternative FAQ

## Is Kortix open source?

Yes. Kortix is the open-source AI Operating System. The code is public: read it, fork it and audit it at [Kortix on GitHub](https://github.com/kortix-ai/suna).

## Is Eigent open source?

Yes. Eigent describes itself as an open-source Cowork desktop and licenses its repository under Apache 2.0 ([eigent-ai/eigent](https://github.com/eigent-ai/eigent), checked October 2026).

## What is the difference between Kortix and Eigent?

Eigent is a local-first desktop app where agents work on one person's files on their own machine. Kortix is a platform a whole company runs from one git repo: agents, skills, memory and connectors are files you own, each session runs on its own isolated cloud computer, and finished work lands through a change request a person approves.

## Can I self-host Kortix for free?

Yes. Self-host is free, and the stack is one Docker Compose project. You pay only for the compute you point it at and the model keys you bring.

## Which models can Kortix run?

Any model provider with your own keys, or the ChatGPT plan you already pay for. You pick the model per agent, per session or per message.

## Where does Kortix run?

Kortix Cloud, your own VPC, or your own on-prem network. Self-hosted instances run the control plane on your hardware, and agent sessions run on a separate sandbox provider.

## Does Kortix work in Slack and Microsoft Teams?

Yes. The agents run in Slack and Microsoft Teams as well as the web app, the CLI and the API, and a message starts a session whose agent replies in the same thread.

## How does the work get approved?

Session work reaches `main` through a change request you read as a diff before anything merges. Merge is default-deny for agents, and approval gates can hold any tool call until a person approves it.
