# Cloud Deployment Decision Matrix

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Built with mdBook](https://img.shields.io/badge/Built%20with-mdBook-blue)](https://rust-lang.github.io/mdBook/)

A decision matrix and guide for evaluating Public Cloud, Private Cloud (hosted/on-prem), and traditional On-Premises infrastructure based on 14 criteria including costs, compliance, scalability, and architecture fit.

## Overview
This guide provides a structured approach to one of the most critical decisions in IT infrastructure: where to deploy your applications. It includes:

- **4 Deployment Models**: Public Cloud, Private Cloud (Hosted), Private Cloud (On-Premises), and Traditional On-Premises
- **14 Evaluation Criteria**: From compliance and costs to scalability and architecture fit
- **Visual Decision Matrix**: Easy-to-understand ratings for quick comparison
- **Detailed Explanations**: In-depth analysis of each criterion
- **Architecture Guidance**: How different application architectures (cloud-native, legacy, etc.) influence the decision

## Who Should Use This Guide?

- **Enterprise Architects** evaluating infrastructure strategies
- **IT Decision Makers** planning cloud migrations or modernization
- **CTOs and IT Directors** making strategic infrastructure investments
- **Solution Architects** designing deployment architectures
- **Consultants** advising clients on infrastructure decisions

## View Online in github

[Decision Matrix](https://github.com/MrThOMaR/cloud-deployment-decision-matrix/blob/main/docs/decision-matrix/en/src/decision-matrix.md)

## Build Locally

If you want to build and view the guide locally:

1. Install [mdBook](https://rust-lang.github.io/mdBook/):
```bash
   cargo install mdbook
```

2. Clone this repository:
```bash
   git clone https://github.com/MrThOMaR/cloud-deployment-decision-matrix.git
```

3. Select your language (English as example)
```bash
   cd cloud-deployment-decision-matrix/docs/decision-matrix/en
```

4. Serve the book locally:
```bash
   mdbook serve --open
```

The guide will open in your browser at `http://localhost:3000`

## Structure
```
📁 cloud-deployment-decision-matrix/docs/decision-matrix/
├── 📁 en/
│   ├── 📄 book.toml              # mdBook configuration
│   └── 📁 src/
│       ├── 📄 SUMMARY.md         # Table of contents
│       ├── 📄 definition-of-cloud-models.md       # Cloud model definitions
│       ├── 📄 decision-matrix.md                  # Decision matrix
│       └── 📄 explanations-of-criteria.md         # Detailed criteria
└── 📁 integrations/
    └── 📁 mcda/
        ├── 📄 README.md          # Integration guide
        └── 📄 mcda-config.json   # MCDA tool configuration
```
## Key Features

### Decision Matrix

The core of this guide is a **14-criteria evaluation matrix** that rates each deployment option:

| Criterion          | Public Cloud | Private Cloud (Hosted) | Private Cloud (On-Prem) | On-Prem (Traditional) |
| ------------------ | ------------ | ---------------------- | ----------------------- | --------------------- |
| Scalability        | ★★★          | ★★★                    | ★★☆                     | ★☆☆                   |
| Security & Control | ★★☆          | ★★★                    | ★★★                     | ★★★                   |
| Cost (TCO)         | ☆☆☆          | ☆☆☆                    | ☆☆☆                     | ☆☆☆                   |
| ...                | ...          | ...                    | ...                     | ...                   |

### Architecture Guidance

Special focus on how application architecture influences deployment decisions:
- **Cloud-Native** (Microservices, Containers, Serverless)
- **Modern Enterprise** (Spring Boot, .NET Core, REST APIs)
- **Traditional Application Servers** (JavaEE, WebSphere, Monoliths)
- **Legacy Systems** (Mainframes, Hardware-dependent)

## Integrations
### Multi-Criteria Decision Analysis

> This Multi-Criteria Decision Analysis (MCDA) tool was designed and developed by Dr. Sven-Erik Willrich — a professional-grade decision analysis framework built on rigorous quantitative methods, designed to transform complex multi-criteria decisions into structured, transparent, and defensible outcomes.
>
> — [Dr. Sven-Erik Willrich, MCDA Framework](https://svenwillrich.de/mcda/)

We provide a ready-to-use configuration file for the MCDA tool. See [integrations/mcda/](docs/decision-matrix/integrations/mcda/) for:
- Pre-configured criteria weights
- Decision alternatives setup
- Usage instructions

## Contributing

Contributions are welcome! This is a living document that benefits from real-world experience and diverse perspectives.

### Contribution Ideas

- Add real-world case studies
- Improve criteria explanations
- Fix typos or improve clarity
- Translate to other languages

## License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

**You are free to:**
- **Share** — copy and redistribute the material
- **Adapt** — remix, transform, and build upon the material

**Under the following terms:**
- **Attribution** — You must give appropriate credit and indicate if changes were made

See [LICENSE](LICENSE) file for details.

## Acknowledgments

1. This decision matrix was developed with assistance from Claude (Anthropic) for structuring content, research, and documentation.
2. Translations were done with assistance from DeepL.

All decisions, evaluations, and final content review were done by [Martin Thorn](https://github.com/MrThOMaR).

## Contact

Have questions or suggestions? Feel free to:
- Open an [Issue](https://github.com/MrThOMaR/cloud-deployment-decision-matrix/issues)
- Start a [Discussion](https://github.com/MrThOMaR/cloud-deployment-decision-matrix/discussions)
- Submit a Pull Request

---

⭐ If you find this guide helpful, please consider giving it a star on GitHub!
