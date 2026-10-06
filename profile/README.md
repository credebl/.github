## ![CREDEBL Logo](https://github.com/credebl/.github/raw/main/logo.svg)

# CREDEBL

[![LFX Health Score](https://insights.linuxfoundation.org/api/badge/health-score?project=credebl)](https://insights.linuxfoundation.org/project/credebl) [![LFX Contributors](https://insights.linuxfoundation.org/api/badge/contributors?project=credebl)](https://insights.linuxfoundation.org/project/credebl) [![LFX Active Contributors](https://insights.linuxfoundation.org/api/badge/active-contributors?project=credebl)](https://insights.linuxfoundation.org/project/credebl)

CREDEBL is an open source, population-scale platform for **Decentralized Identity (DID)** and **Verifiable Credentials (VC)** management, and a project of the [Linux Foundation Decentralized Trust](https://www.lfdecentralizedtrust.org).

[Website](https://credebl.id) · [Documentation](https://docs.credebl.id) · [LFDT project page](https://www.lfdecentralizedtrust.org/projects/credebl)

## What is CREDEBL?

Verifiable credentials let an organization issue a digital credential — a diploma, a licence, a national ID — that anyone can cryptographically verify, and that the holder controls and shares selectively. Building this end to end normally means assembling agents, ledgers, DID methods, credential formats, and wallet software yourself.

CREDEBL is the reusable core that removes that work. It provides scalable services for issuing, holding, and verifying credentials, so teams can build Self-Sovereign Identity (SSI) solutions without rebuilding the plumbing for every use case.

The platform is **multi-tenant, agent-agnostic, and ledger-agnostic** — it works across different Verifiable Data Registries, DID methods, and credential formats, including ledger-less issuance via `did:web`, `did:key`, and `did:peer`. It is built on a micro-services architecture and scales from a proof of concept to national deployments.

CREDEBL is a **Digital Public Good**, approved by the UN-endorsed DPG Alliance. Visit the [CREDEBL DPG page](https://www.digitalpublicgoods.net/r/credebl) in the DPG registry.


## Projects

CREDEBL is made up of several components. Most people start with the **Core SSI Platform**; everything else builds on it.

| Repository | What it is |
|---|---|
| [**platform**](https://github.com/credebl/platform) | **Start here.** The core SSI backend — issuance, verification, DIDs, schemas, agents, and APIs. |
| [**studio**](https://github.com/credebl/studio) | Web user interface for the platform: manage organizations, schemas, credentials, and connections without writing code. |
| [**mobile-sdk**](https://github.com/credebl/mobile-sdk) | The Mobile Wallet SDK — a React-Native SSI edge-wallet SDK, built on Credo, for building your own wallet app. |
| [**mobile-wallet**](https://github.com/credebl/mobile-wallet) | The reference SSI wallet app, built on OpenWallet Foundation Bifold, for building and testing your wallet. |
| [**webauthn-server**](https://github.com/credebl/webauthn-server) | WebAuthn server adding FIDO Passkeys support for passwordless authentication. |
| [**governance**](https://github.com/credebl/governance) | The project's technical charter and organization-wide repository configuration. |

## Where CREDEBL is used

CREDEBL runs in production at national scale, including as the credential layer for the [**Royal Government of Bhutan's National Digital Identity (NDI)**](https://www.bhutanndi.com) and [**Papua New Guinea's SevisPass Digital ID**](https://www.biometricupdate.com/202410/papua-new-guinea-advances-digital-id-wallet-and-govt-platform-to-pilot). It also powers the [**Sovio.id**](https://sovio.id) platform by AYANWORKS.

Beyond citizen identity, it has been applied across healthcare, financial services, education, and government services — anywhere credentials need to be issued once and verified repeatedly without a central authority mediating every check.

## Getting started

The fastest path depends on what you're trying to do:

- **Evaluate the platform** — follow the setup guide in [docs.credebl.id](https://docs.credebl.id) to run the stack locally.
- **Run the backend** — see the [platform repository](https://github.com/credebl/platform) for prerequisites (Docker, PostgreSQL, NATS) and service startup.
- **Explore through a UI** — pair the platform with [Studio](https://github.com/credebl/studio).
- **Build a wallet** — start from the [Mobile SDK](https://github.com/credebl/mobile-sdk), and use the [reference Mobile Wallet app](https://github.com/credebl/mobile-wallet) to build and test.

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

Contribution guidelines are in the `CONTRIBUTING.md` files of the [platform](https://github.com/credebl/platform) and [studio](https://github.com/credebl/studio) repositories. The project's technical charter is in the [governance repository](https://github.com/credebl/governance).

## Community meetings

CREDEBL community calls are open to everyone. They are a good place to ask questions, discuss roadmap priorities, and learn how to contribute.

| Meeting | Calendar Link |
|---|---|
| CREDEBL Community Call | https://zoom-lfx.platform.linuxfoundation.org/meetings/credebl?view=month |

Past meeting recordings, along with demos, walkthroughs, and talks, are available on the [CREDEBL YouTube playlist](https://www.youtube.com/playlist?list=PL0MZ85B_96CHvUkCiy8mZF1DdxY4dKVYm).

## Community

- **Chat and updates:** [LFDT Discord](https://discord.lfdecentralizedtrust.org) `#credebl` | [Twitter](https://twitter.com/credebl)
- **Help, feature requests, and bugs:** [GitHub Discussions](https://github.com/orgs/credebl/discussions) | [docs.credebl.id](https://docs.credebl.id)

## Project status

CREDEBL is an **incubating** project at LF Decentralized Trust. It was created by [AYANWORKS](https://ayanworks.com) and released as open source in 2023, and contributed to LFDT in 2025. The platform is production-proven, and the community is focused on growing participation, broadening ledger and credential-format support, and improving documentation and onboarding.

## Credits

CREDEBL builds on the work of several open source projects, including Hyperledger Aries, Credo, Bifold, Askar, and Indy.
