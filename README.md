# Sapio State

Sapio State is an open-source research repository for a proposed transnational digital polity. It documents hypotheses about expert-informed governance, local-first civic infrastructure, open-source rulemaking, privacy-preserving identity, funding models, mobility agreements, and technology programmes.

This repository is a design study, not a recognized sovereign state. It does not create nationality, territorial rights, diplomatic status, tax status, visa rights, or immunity from the law of any country.

## Concepts under study

- **Sapiocracy**: route a concrete decision to people with relevant demonstrated expertise, while retaining rights constraints, conflict-of-interest rules, public review, and appeal.
- **Rules as software**: maintain human-readable rules alongside machine-readable policy, tests, version history, rationale, and simulations.
- **Passport**: a portable cryptographic residency/identity credential that is not locked to one device.
- **Local-first / P2P**: keep personal data under user control and exchange the minimum information needed for a transaction.
- **No general compulsory tax**: a funding hypothesis to test against fees, endowments, voluntary contributions, commercial activity, and commons-management charges.
- **Resident token**: a possible initial allocation to new residents; monetary, regulatory, governance, and abuse questions remain open.
- **Global mobility**: a long-term goal that would require agreements with existing states.
- **Technology programmes**: research tracks such as advanced AI, fusion energy, e-government, privacy infrastructure, communications, and manufacturing.

## Territory

The proposal uses Earth as its global scope of concern. This is not a claim of territorial ownership or jurisdiction over existing states.

Any future formal legal status would depend on lawful recognition, agreements, and the domestic and international law applicable to the participating parties.

## AGENT and Agent OS

The proposed [AGENT](https://github.com/alex-mextner/AGENT) wrist computer can host a Passport credential, but residency identity must remain portable across devices.

The computing layer references [Agent OS](https://agentos-bible.vercel.app/) and its [source repository](https://github.com/alex-mextner/AgentOS): app-last, local-first, agent-native software with durable entities and explicit capabilities.

## Documents

- [Governance / sapiocracy](GOVERNANCE.md)
- [Legal reality and interfaces](docs/legal-reality.md)
- [Privacy and security](docs/privacy-security.md)
- [Economy and commons](docs/economy.md)
- [Passport and residency](docs/passport.md)
- [Technology programmes](docs/technology.md)
- [Ratification and mobility roadmap](docs/ratification-roadmap.md)
- [Need matching / hyper-targeting](docs/hyper-targeting.md)

## Status

Early concept. The repository is intended to make assumptions explicit and testable before any institutional claim is made.

## Private-topology check

CI runs `scripts/check-private-topology.sh` (plus gitleaks) on every pull request to keep private addresses, host names, MAC addresses and e-mails out of tracked files; use placeholders such as `<server-lan-ip>` or `<tailnet-host>` instead. To also catch your own machine names locally, list one regular expression per line in `~/.config/private-topology/denylist.txt` (never committed) and run the script before pushing.
