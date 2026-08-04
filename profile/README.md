## ![CREDEBL Logo](https://github.com/credebl/.github/raw/main/logo.svg)

# CREDEBL

CREDEBL is an open source, population-scale platform for **Decentralized Identity (DID)** and **Verifiable Credentials (VC)** management, and a project of the [Linux Foundation Decentralized Trust](https://www.lfdecentralizedtrust.org).

[Website](https://credebl.id) · [Documentation](https://docs.credebl.id) · [LFDT project page](https://www.lfdecentralizedtrust.org/projects/credebl)

## What is CREDEBL?

Verifiable credentials let an organization issue a digital credential — a diploma, a licence, a national ID — that anyone can cryptographically verify, and that the holder controls and shares selectively. Building this end to end normally means assembling agents, ledgers, DID methods, credential formats, and wallet software yourself.

CREDEBL is the reusable core that removes that work. It provides scalable services for issuing, holding, and verifying credentials, so teams can build Self-Sovereign Identity (SSI) solutions without rebuilding the plumbing for every use case.

The platform is **multi-tenant, agent-agnostic, and ledger-agnostic** — it works across different Verifiable Data Registries, DID methods, and credential formats, including ledger-less issuance via `did:web`, `did:key`, and `did:peer`. It is built on a micro-services architecture and scales from a proof of concept to national deployments.

CREDEBL is a **Digital Public Good**, approved by the UN-endorsed DPG Alliance.

## Projects

CREDEBL is made up of several components. Most people start with the **Core SSI Platform**; everything else builds on it.

| Repository | What it is |
|---|---|
| [**platform**](https://github.com/credebl/platform) | **Start here.** The core SSI backend — issuance, verification, DIDs, schemas, agents, and APIs. |
| [**studio**](https://github.com/credebl/studio) | Web user interface for the platform: manage organizations, schemas, credentials, and connections without writing code. |
| [**adeya-wallet**](https://github.com/credebl/adeya-wallet) | The SSI edge wallet app and SDK that credential holders use. |
| [**webauthn-server**](https://github.com/credebl/webauthn-server) | WebAuthn server adding FIDO Passkeys support for passwordless authentication. |
| [**governance**](https://github.com/credebl/governance) | Governance documents and organization-wide repository configuration. |

## Where CREDEBL is used

CREDEBL runs in production at national scale, including as the credential layer for **Bhutan's National Digital Identity (NDI)** and **Papua New Guinea's SevisPass Digital ID**.

Beyond citizen identity, it has been applied across healthcare, financial services, education, and government services — anywhere credentials need to be issued once and verified repeatedly without a central authority mediating every check.

## Getting started

The fastest path depends on what you're trying to do:

- **Evaluate the platform** — follow the setup guide in [docs.credebl.id](https://docs.credebl.id) to run the stack locally.
- **Run the backend** — see the [platform repository](https://github.com/credebl/platform) for prerequisites (Docker, PostgreSQL, NATS) and service startup.
- **Explore through a UI** — pair the platform with [Studio](https://github.com/credebl/studio).
- **Build a wallet** — start from the [ADEYA Wallet](https://github.com/credebl/adeya-wallet) app and SDK.

<!-- TODO: consider linking a single "quickstart in 10 minutes" page here once one exists -->

## Roadmap

Current and near-term work is tracked on the [public roadmap](https://github.com/orgs/credebl/projects/5).

## Contributing

CREDEBL welcomes developers, identity practitioners, implementers, and organizations working on decentralized identity. Contributions are not limited to code — documentation, examples, issue triage, and deployment reports are all valuable.

Good ways to get started:

1. Read the [documentation](https://docs.credebl.id) and get the platform running locally.
2. Browse open issues in the [platform repository](https://github.com/credebl/platform), especially anything labelled `good first issue`.
3. Introduce yourself on the `#credebl` channel on [LFDT Discord](https://discord.lfdecentralizedtrust.org).
4. Discuss designs in [GitHub Discussions](https://github.com/orgs/credebl/discussions) before starting work.

**For larger changes, please open an issue first** so maintainers and the community can discuss the approach before implementation.

Contribution guidelines and governance materials live in the [governance repository](https://github.com/credebl/governance).

## Community meetings

CREDEBL community calls are open to everyone. They are a good place to ask questions, discuss roadmap priorities, and learn how to contribute.

| Meeting | Calendar Link |
|---|---|
| CREDEBL Community Call | https://zoom-lfx.platform.linuxfoundation.org/meeting/95415588760?password=bee3e742-10db-4224-8991-d61053249ce9 |

Past meeting recordings and presentations can be accessed through:

- [LFX Individual Dashboard](https://openprofile.dev/)
- [LFDT Meeting Calendar](https://zoom-lfx.platform.linuxfoundation.org/meetings/lf-decentralized-trust)

## Community

- **Chat and updates:** [LFDT Discord](https://discord.lfdecentralizedtrust.org) `#credebl` | [Twitter](https://twitter.com/credebl)
- **Help, feature requests, and bugs:** [GitHub Discussions](https://github.com/orgs/credebl/discussions) | [docs.credebl.id](https://docs.credebl.id)
- **Videos:** demos, walkthroughs, and talks on the [CREDEBL YouTube playlist](https://www.youtube.com/playlist?list=PL0MZ85B_96CHvUkCiy8mZF1DdxY4dKVYm)

## Project status

CREDEBL is an **incubating** project at LF Decentralized Trust. It was created by [AYANWORKS](https://ayanworks.com) and released as open source in 2023, and contributed to LFDT in 2025. The platform is production-proven, and the community is focused on growing participation, broadening ledger and credential-format support, and improving documentation and onboarding.

## Credits

CREDEBL builds on the work of several open source projects, including Hyperledger Aries, Bifold, Askar, and Indy.