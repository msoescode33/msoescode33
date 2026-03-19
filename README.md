# Michael: Security Engineer

Cloud security and DevSecOps engineer with hands-on depth across Azure, CrowdStrike, and CI/CD security automation. I build reproducible, evidence-based security systems, pipeline gates that block real threats, detection rules that fire on real behaviour, and infrastructure guardrails that enforce policy before deployment.

---

## Portfolio - DevSecOps Deploy-n-Show

Ten end-to-end security engineering projects. Each runs `make demo` from a clean clone. Each produces real pipeline output, real tool findings, and real enforcement decisions.

**[→ View the full repository](https://github.com/msoescode33/DevSecOps-Deploy-n-Show)**

| Project | What it does |
|---|---|
| **P01: IaC Guardrails** | Terraform + Checkov two-gate pipeline. Secrets detection via Gitleaks, policy enforcement via Checkov. Intentional misconfigurations included to validate controls fire. |
| **P02: Kubernetes Baseline** | KIND cluster with Kyverno admission control and Trivy image scanning. Intentional policy violations by design — controls are verified to work, not assumed. |
| **P03: Container Supply Chain** | SBOM generation via Syft, keyless image signing via Cosign/Sigstore, OCI-attached signature stored in GHCR. Tamper-evident provenance end-to-end. |
| **P05: Multi-Gate CI Pipeline** | Four independent jobs: SAST (Semgrep), SCA (pip-audit), secrets detection (Gitleaks), IaC scanning (Checkov). Discrete pass/fail per gate, named artifacts, SARIF output. |
| **P07: Policy as Code** | OPA + Conftest enforcing custom Rego policies as a CI gate. Per-gate job structure, dynamic pipeline summary via `needs.<job>.result`. |
| **P08: Runtime Detection** | Five custom Falco rules firing against live container behaviour. Gate 3 uses Python/PyYAML structural validation. Outbound connection rules scoped to avoid false positives. |

---

## Azure Security (Azure Repos + Defender for Cloud + Azure DevOps))

> A second portfolio series focused entirely on Microsoft-native security
> tooling — Bicep, Azure DevOps Pipelines, Defender for Cloud, Azure Policy,
> and Entra ID. Where DevSecOps-Deploy-n-Show demonstrates open-source
> security tooling on GitHub Actions, this series demonstrates the same
> engineering discipline using the Microsoft security stack.

| Project | Focus | Stack |
|---|---|---|
| P01: ACA Defender Posture | Container security · Defender for Containers · Azure Policy as code | Bicep · ADO · ACA · ACR · Defender for Cloud |
| P02: Defender for DevOps | Pipeline findings in Defender for Cloud · MSDO · repo-wide SAST/IaC scanning | Bicep · ADO · MicrosoftSecurityDevOps task |
| P03: Policy as Code | Custom policy initiatives · Deny effect · compliance automation · remediation tasks | Terraform · ADO · Azure Policy |
| P04: Defender for Storage | Blob threat detection · malware scanning · end-to-end alert evidence | Bicep · ADO · Defender for Storage · EICAR simulation |
| P05: Entra ID Posture | Conditional Access as code · PIM JIT access · Identity Secure Score | Bicep · Graph API · ADO · Entra ID |

**Common patterns across all projects:**
- Every security control is codified
- Each project includes full evidence collection (CLI output, portal screenshots, pipeline logs)
- Sensitive identifiers redacted for public consumption
- Docs include architecture decisions, threat model, runbook, and interview notes

---

## Core Tooling

`Azure` `Defender for Cloud` `Microsoft Sentinel` `CrowdStrike Falcon` `Terraform` `Checkov` `GitHub Actions` `Gitleaks` `Semgrep` `Syft` `Cosign` `Kyverno` `Trivy` `Falco` `OPA/Conftest` `Docker` `Kubernetes` `Python` `Linux` `Azure DevOps`

---

## TryHackMe

[![TryHackMe](tryhackme.png)](https://tryhackme.com/p/GooseyintheShell)
