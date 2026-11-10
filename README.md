# Awesome-CI-CD-Pipeline-Build-Integrations

# Top CI/CD Pipeline & Build Integrations Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Continuous Integration, Continuous Delivery & Automated Build Orchestration*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **CI/CD Pipeline & Build Integrations**. These tools help development teams automate the build, test, and deployment lifecycle—covering hosted runners, pipeline orchestration engines, and self-hosted CI servers that integrate with version control, testing frameworks, and cloud infrastructure.

**Examples** include Postman CI Integrations, GitHub Actions, GitLab CI/CD, CircleCI, Jenkins, Travis CI, Bitbucket Pipelines, AWS CodePipeline, Azure Pipelines, and TeamCity (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted CI servers, open-source pipeline frameworks, and community-maintained runner images—ideal for DevOps engineers, platform teams, and developers building transparent, vendor-neutral build automation without per-minute cloud billing surprises.

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Postman CI Integrations](https://www.postman.com/)** | API platform with native CI integrations for running Postman collections via Newman in GitHub Actions, Jenkins, GitLab CI, CircleCI, Azure DevOps, and Bitbucket Pipelines. Enables automated API testing as a pipeline stage. | Free plan (single user); paid plans from $14/user/month (Basic)  | Free plan: single user only (team collaboration removed March 2026), limited monitoring and mock calls  |
| **[GitHub Actions](https://github.com/features/actions)** | Native CI/CD within GitHub with 20,000+ Marketplace actions; supports matrix builds, reusable workflows, and self-hosted runners. Public repositories get unlimited free minutes on all runner types. | $0 for public repos; private repos beyond included minutes billed per-minute (Linux ~$0.008/min)  | Free plan: 2,000 minutes/month for private repos (Linux 1x multiplier; macOS 10x); public repos unlimited and free  |
| **[GitLab CI/CD](https://about.gitlab.com/)** | Integrated CI/CD within GitLab with `.gitlab-ci.yml` pipeline definitions, Auto DevOps, and Kubernetes integration. Self-hosted runners consume zero minutes on any tier. | Free: $0; Premium: $29/user/month (10,000 compute minutes/group)  | Free tier: 400 compute minutes/month per top-level namespace, 5 users/namespace, unlimited self-hosted runners  |
| **[CircleCI](https://circleci.com/)** | Cloud CI/CD platform with orbs for reusable configuration, Docker layer caching, and test splitting. Supports Docker, Linux VM, macOS, Windows, and GPU executors. | Performance: $15/month base + credits; Scale: custom  | Free plan: 30,000 credits/month (~3,000 Linux medium minutes), 5 active users, 5 self-hosted runners, 1 macOS concurrency  |
| **[Jenkins](https://www.jenkins.io/)** | Self-hosted automation server with 1,800+ plugins covering virtually every tool and cloud. The most flexible CI engine, but requires infrastructure provisioning and ongoing maintenance. | Free software (MIT); infrastructure costs $30–80/month for a small VM plus operator time  | No hosted free tier—software is free, but you pay for servers and maintenance (estimated 4–12 hrs/month operator time)  |
| **[Travis CI](https://www.travis-ci.com/)** | Cloud CI with simple `.travis.yml` configuration; historically popular for open-source projects. Supports Linux, macOS, and Windows builds. | Usage Based: $15/month (35,000 Linux build credits, 80 concurrent jobs)  | Free trial: 14-day credit allotment (one-time, non-renewable); open-source projects eligible for free OSS plan credits  |
| **[Bitbucket Pipelines](https://bitbucket.org/product/features/pipelines)** | Integrated CI/CD within Bitbucket with YAML configuration and Docker support. Self-hosted runners free up to 100 per workspace. | Standard: $3/user/month; Premium: $6/user/month  | Free plan: 5 users, 50 build minutes/month; additional minutes $10 per 1,000  |
| **[AWS CodePipeline](https://aws.amazon.com/codepipeline/)** | Managed continuous delivery service orchestrating build, test, and deploy stages across AWS and third-party services. V1 pipelines billed per active pipeline; V2 per action execution minute. | V1: $1.00/active pipeline/month; V2: $0.002/action-execution-minute  | AWS Free Tier: 1 free active V1 pipeline/month; 100 free V2 action-execution minutes/month  |
| **[Azure Pipelines](https://azure.microsoft.com/en-us/products/devops/pipelines/)** | Microsoft's CI/CD service within Azure DevOps with YAML pipelines, hosted and self-hosted agents, and deep Azure integration. Public projects get 10 free parallel jobs. | $40/month per extra Microsoft-hosted parallel job; $15/month per extra self-hosted job  | Free tier: 1 Microsoft-hosted job with 1,800 minutes/month + 1 self-hosted job with unlimited minutes; public projects: 10 free parallel jobs  |
| **[TeamCity](https://www.jetbrains.com/teamcity/)** | JetBrains' CI server with on-premises and cloud editions. Professional edition is free forever; Enterprise adds unlimited build configurations and agents. | Professional: free forever; Enterprise: from $1,999/year  | Professional (on-premises): free forever, unlimited users, 3 build agents, 100 build configurations, 10 pipelines  |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[ci-matrix-starter](https://github.com/CoderDeltaLAN/ci-matrix-starter)** | [![Stars](https://img.shields.io/github/stars/CoderDeltaLAN/ci-matrix-starter?style=social&color=white)](https://github.com/CoderDeltaLAN/ci-matrix-starter/stargazers) | Lean, production-ready GitHub Actions starter with reusable CI workflows for Python (3.11/3.12) and TypeScript/Node 20. Includes CodeQL, optional SBOM, Dependabot auto-merge, and release drafter for always-green CI. |
| **[pygha](https://github.com/CoderDeltaLAN/pygha)** | [![Stars](https://img.shields.io/github/stars/CoderDeltaLAN/pygha?style=social&color=white)](https://github.com/CoderDeltaLAN/pygha/stargazers) | Python-native CI/CD framework for defining, testing, and transpiling pipelines to GitHub Actions YAML. Jobs defined as Python functions with `@job` decorator and `depends_on` for sequential stages. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[RunWright](https://github.com/marketplace/actions/runwright)** | [![Stars](https://img.shields.io/github/stars/runwright/runwright?style=social&color=white)](https://github.com/runwright/runwright/stargazers) | Free GitHub Action that auto-scales runners based on actual test load, enabling dynamic parallelism with upfront duration targets. |
| **[BrowserStack Quality Gate](https://github.com/marketplace/actions/browserstack-quality-gate)** | — | Quality gate action providing results from BrowserStack Quality Gate API to reduce flaky test noise in CI pipelines. |
| **[playwright-load-balancer](https://github.com/marketplace/actions/playwright-load-balancer)** | — | Dynamically scales GitHub runners based on changed test files or test count, using Playwright sharding for distribution. |

**Frameworks for building custom systems**: Combine **ci-matrix-starter** for reusable GitHub Actions workflows, **pygha** for Python-native pipeline definition and transpilation, and **RunWright** for dynamic parallel test scaling—integrated with self-hosted runners or cloud CI for cost-optimized execution.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- CI/CD platforms handle source code, credentials, and deployment access; enforce least-privilege runner permissions, mask secrets in logs, and isolate self-hosted runners.
- Pricing and free-tier limits change frequently; always verify against the vendor's current pricing page before making architectural decisions.

---

**Made for DevOps engineers, platform teams, QA architects, and developers building reliable build pipelines.**  
Let's make CI/CD pipeline integration more open, automatable, and observable.
