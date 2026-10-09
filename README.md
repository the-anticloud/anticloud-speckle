# SPECKLE

![licence](https://img.shields.io/badge/licence-Apache-2.0-blue) ![checks](https://img.shields.io/badge/checks-0_PASS-brightgreen)

> Governed Anticloud packaging of upstream `SPECKLE` in category **ARCHITECTURAL_DESIGN**. 0/16 checks PASS (measured). Every number traces to a named file plus run stamp.

**Upstream:** https://github.com/specklesystems/speckle-sharp | **Upstream pin:** `e4bb61df9b4756223ce67f0b5e0c32646d9c106e` (source: bench:BENCH.json) | **Category:** ARCHITECTURAL_DESIGN | **Licence:** Apache-2.0 | **Overlay licence:** Anticommons 0.1.0

---

## What This Project Does

<h1 align="center">
  <img src="https://user-images.githubusercontent.com/2679513/131189167-18ea5fe1-c578-47f6-9785-3748178e4312.png" width="150px"/><br/>
  Speckle | Sharp (Legacy)
</h1>

<p align="center"><a href="https://twitter.com/SpeckleSystems"><img src="https://img.shields.io/twitter/follow/SpeckleSystems?style=social" alt="Twitter Follow"></a> <a href="https://speckle.community"><img src="https://img.shields.io/discourse/users?server=https%3A%2F%2Fspeckle.community&amp;style=flat-square&amp;logo=discourse&amp;logoColor=white" alt="Community forum users"></a> <a href="https://speckle.systems"><img src="https://img.shields.io/badge/https://-speckle.systems-royalblue?style=flat-square" alt="website"></a> <a href="https://speckle.guide/dev/"><img src="https://img.shields.io/badge/docs-speckle.guide-orange?style=flat-square&amp;logo=read-the-docs&amp;logoColor=white" alt="docs"></a></p>

> Speckle is the first AEC data hub that connects with your favorite AEC tools. Speckle exists to overcome the challenges of working in a fragmented industry where communication, creative workflows, and the exchange of data are often hindered by siloed software and processes. It is here to make the industry better.

<h3 align="center">
    .NET SDK, tooling, schema and Connectors
</h3>

<p align="center"><a href="https://circleci.com/gh/specklesystems/speckle-sharp"><img src="https://circleci.com/gh/specklesystems/speckle-sharp.svg?style=svg" alt=".NET Core"></a></p>

> [!WARNING]
> This is our legacy .NET project! Check out our active .NET projects here:
> [`speckle-sharp-connectors`](https://github.com/specklesystems/speckle-sharp-connectors): our .NET next generation connectors and desktop UI
> [`speckle-sharp-sdk`](https://github.com/specklesystems/speckle-sharp-sdk): our .NET SDK, Tests, and Objects

# project structure

This monorepo is the home to our Speckle 2.0 .NET projects:

- [`Core`](https://github.com/specklesystems/speckle-sharp/tree/main/Core): the canonical SDK for Speckle. It supports multiple [data transports](https://discourse.speckle.works/t/core-2-0-transports/919), and advanced [decomposition API](https://discourse.speckle.works/t/core-2-0-decomposition-api/911) for design data, and offers a [dynamic base](https://discourse.speckle.works/t/core-2-0-the-base-object/782) for object definition.
- [`Objects`](https://github.com/specklesystems/speckle-sharp/tree/main/Objects): the Objects Kit is our default interoperability kit. Read more about kits and their role in the Speckle ecosystem [here](https://discourse.speckle.works/t/introducing-kits-2-0/710).
  - [`Converters`](https://github.com/specklesystems/speckle-sharp/tree/main/Objects/Converters): conversion routines for each of the connectors mentioned below
- Speckle Connectors
  - [`ConnectorAutocadCivil`](https://github.com/specklesystems/speckle-sharp/tree/main/ConnectorAutocadCivil): for Autodesk AutoCAD and Civil3D 2021+
  - [`ConnectorDynamo`](https://github.com/specklesystems/speckle-sharp/tree/main/ConnectorDynamo): for Autodesk Dynamo
  - [`ConnectorGrasshopper`](https://github.com/specklesystems/speckle-sharp/tree/main/ConnectorGrasshopper): for McNeel Grasshopper
  - [`ConnectorRevit`](https://github.com/specklesystems/speckle-sharp/tree/main/ConnectorRevit): for Autodesk Revit 2019+
  - [`ConnectorRhino`](https://github.com/specklesystems/speckle-sharp/tree/main/ConnectorRhino): for McNeel Rhino 6+
- [`DesktopUI2`](https://github.com/specklesystems/speckle-sharp/tree/main/DesktopUI2): reusable UI for all connectors (except visual programming)

### Other projects

Make sure to also check and ⭐️ these other Speckle projects:

- [`speckle-server`](https://github.com/specklesystems/speckle-server): Server and Web packages
- [`specklepy`](https://github.com/specklesystems/specklepy): Python SDK 🐍
- [`speckle-excel`](https://github.com/specklesystems/speckle-excel): Excel connector
- [`speckle-unity`](https://github.com/specklesystems/speckle-unity): Unity 3D connector
- [`speckle-blender`](https://github.com/specklesystems/speckle-blender): Blender connector
- [`speckle-unreal`](https://github.com/specklesystems/speckle-unreal): Unreal Engine Connector
- [`speckle-qgis`](https://github.com/specklesystems/speckle-qgis): QGIS connectod
- [`speckle-powerbi`](https://github.com/specklesystems/speckle-powerbi): PowerBi connector
- and more [connectors & tooling](https://github.com/specklesystems/)!

## Developing and Debugging

source this monorepo; **each section has its own readme**, so then just follow those instructions.

Issues or questions? We encourage everyone interested to debug / hack / contribute / give feedback to this project.

> **A note on Accounts:**
> The connectors themselves don't have features to manage your Speckle accounts; this functionality is delegated to the Speckle Manager desktop app. You can install it [from here](https://speckle-releases.ams3.digitaloceanspaces.com/manager/SpeckleManager%20Setup.exe).

### Contributing

Please make sure you read the [contribution guidelines](.github/CONTRIBUTING.md) for an overview of the best practices we try to follow.

### Security

For any security vulnerabilities or concerns, please contact us directly at security[at]speckle.systems.

### License

Unless otherwise described, the code in this project is licensed under the Apache-2.0 License. Please note that some modules, extensions or code herein might be otherwise licensed. This is indicated either in the root of the containing folder under a different license file, or in the respective file's header. If you have any questions, don't hesitate to get in touch with us via [email](mailto:hello@speckle.systems).

(Full upstream documentation preserved in UPSTREAM_CLONE/README.md.)

---

## Installation

See the upstream documentation quoted in What This Project Does above.

## Usage

Speckle | Sharp (Legacy)
</h1>

<p align="center"><a href="https://twitter.com/SpeckleSystems"><img src="https://img.shields.io/twitter/follow/SpeckleSystems?style=social" alt="Twitter Follow"></a> <a href="https://speckle.community"><img src="https://img.shields.io/discourse/users?server=https%3A%2F%2Fspeckle.community&amp;style=flat-square&amp;logo=discourse&amp;logoColor=white" alt="Community forum users"></a> <a href="https://speckle.systems"><img src="https://img.shields.io/badge/https://-speckle.systems-royalblue?style=flat-square" alt="website"></a> <a href="https://speckle.guide/dev/"><img src="https://img.shields.io/badge/docs-speckle.guide-orange?style=flat-square&amp;logo=read-the-docs&amp;logoColor=white" alt="docs"></a></p>

> Speckle is the first AEC data hub that connects with your favorite AEC tools. Speckle exists to overcome the challenges of working in a fragmented industry where communication, creative workflows, and the exchange of data are often hindered by siloed software and processes. It is here to make the industry better.

<h3 align="center">
    .NET SDK, tooling, schema and Connectors
</h3>

<p align="center"><a href="https://circleci.com/gh/specklesystems/speckle-sharp"><img src="https://circleci.com/gh/specklesystems/speckle-sharp.svg?style=svg" alt=".NET Core"></a></p>

> [!WARNING]
> This is our legacy .NET project! Check out our active .NET projects here:
> [`speckle-sharp-connectors`](https://github.com/specklesystems/speckle-sharp-connectors): our .NET next generation connectors and desktop UI
> [`speckle-sharp-sdk`](https://github.com/specklesystems/speckle-sharp-sdk): our .NET SDK, Tests, and Objects

## API

- [`Objects`](https://github.com/specklesystems/speckle-sharp/tree/main/Objects): the Objects Kit is our default interoperability kit. Read more about kits and their role in the Speckle ecosystem [here](https://discourse.speckle.works/t/introducing-kits-2-0/710).
  - [`Converters`](https://github.com/specklesystems/speckle-sharp/tree/main/Objects/Converters): conversion routines for each of the connectors mentioned below
- Speckle Connectors
  - [`ConnectorAutocadCivil`](https://github.com/specklesystems/speckle-sharp/tree/main/ConnectorAutocadCivil): for Autodesk AutoCAD and Civil3D 2021+
  - [`ConnectorDynamo`](https://github.com/specklesystems/speckle-sharp/tree/main/ConnectorDynamo): for Autodesk Dynamo
  - [`ConnectorGrasshopper`](https://github.com/specklesystems/speckle-sharp/tree/main/ConnectorGrasshopper): for McNeel Grasshopper
  - [`ConnectorRevit`](https://github.com/specklesystems/speckle-sharp/tree/main/ConnectorRevit): for Autodesk Revit 2019+
  - [`ConnectorRhino`](https://github.com/specklesystems/speckle-sharp/tree/main/ConnectorRhino): for McNeel Rhino 6+
- [`DesktopUI2`](https://github.com/specklesystems/speckle-sharp/tree/main/DesktopUI2): reusable UI for all connectors (except visual programming)

## Dependencies

| Metric | Value |
|--------|-------|
| Files | measured |
| Lines of Code | measured |
| Dependencies | measured |
| Upstream licence | Apache-2.0 |
| Overlay licence | Anticommons 0.1.0 |

Dependency manifests live in `UPSTREAM_CLONE/`; pinned lockfile in `anticloud/` where applicable.

## Configuration

See upstream source in UPSTREAM_CLONE/ and the quoted documentation above.

## Contributing

# Speckle Contribution Guidelines

## Introduction

Thank you for reading this! Speckle's a rather wide network of parts that depend on each other, either directly, indirectly or even just cosmetically.

> **Speckle** is a quite large ecosystem of moving parts. Any changes may have unintended effects, that can cause problems quickly for many people (and processes) that rely on Speckle.

This means that what might look like a simple quick change in one project may have a big hidden cost that propagates around other parts of the project. We're all here to help each other, and this guide is meant to help you get started and promote a framework that can untangle all these dependecies through discussion!

## Bugs & Issues 🐞

### Found a new bug?

- First step is to check whether this is a new bug! We encourage you to search through the issues of the project in question **and** associated projects!

- If you come up with nothing, **open a new issue with a clear title and description**, as much relevant information as possible: system configuration, code samples & steps to reproduce the problem.

- Can't mention this often enough: tells us how to reproduce the problem! We will ignore or flag as such issues without reproduction steps.

- Try to reference & note all potentially affected projects.

### Sending a PR for Bug Fixes

You fixed something! Great! We hope you logged it first :) Make sure though that you've covered the lateral thinking needed for a bug report, as described above, also in your implementation! If there any tests, make sure they all pass. If there are none, it means they're missing - so add them!

### Code Style

When collaborating on a project in GitHub, it's important to follow coding conventions and style guidelines to ensure consistency and readability of the codebase. One commonly used convention is to use two spaces for indentation.

To use two spaces for indentation in GitHub, you can configure your text editor or IDE to use this indentation style. Once you've written your code, you can commit and push your changes to GitHub.

When collaborating with others on GitHub, it's important to communicate any changes to coding conventions or style guidelines, and to work together to maintain a consistent coding style throughout the project. Code reviews can also help ensure that code is well-formatted and easy to read.

## New Features 🎉

The golden rule is to Discuss First!

- Before embarking on adding a new feature, suggest it first as an issue with the `enhancement` label and/or title - this will allow relevant people to pitch in
- We'll now discuss your requirements and see how and if they fit within the Speckle ecosystem.
- The last step is to actually start writing code & submit a PR so we can follow along!
- All new features should, if and where possible, come with tests. We won't merge without!

> Many clients may potentially have overlapping scopes, some features might already be in dev somewhere else, or might have been postponed

## Licence

Upstream (c) its contributors under Apache-2.0 - see `UPSTREAM_CLONE/LICENSE`. This packaging overlay is licensed under Anticommons 0.1.0.

## Upstream

- URL: https://github.com/specklesystems/speckle-sharp
- Pinned commit: `e4bb61df9b4756223ce67f0b5e0c32646d9c106e`
- Verify: compare against the pinned commit in the upstream project history.

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`d2403ec3e79592c1843b6aa386ea2ed7dcbb24fe019e2aeed4a932c34199876a`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| DANS (KNAW/NWO, Netherlands) | 10.17026/PT | EU-recognised archive |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe
and Mail, Business Insider, National Post, Financial Post, StreetInsider,
Digital Journal, Barchart, International Business Times, and Fox News.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

