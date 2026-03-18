# Michael: Security Engineer

Cloud security and DevSecOps engineer with hands-on depth across Azure, CrowdStrike, and CI/CD security automation. I build reproducible, evidence-based security systems, pipeline gates that block real threats, detection rules that fire on real behaviour, and infrastructure guardrails that enforce policy before deployment.

---

## Portfolio — DevSecOps Deploy-n-Show

Ten end-to-end security engineering projects. Each runs `make demo` from a clean clone. Each produces real pipeline output, real tool findings, and real enforcement decisions.

**[→ View the full repository](https://github.com/msoescode33/DevSecOps-Deploy-n-Show)**

| Project | What it does |
|---|---|
| **P01 — IaC Guardrails** | Terraform + Checkov two-gate pipeline. Secrets detection via Gitleaks, policy enforcement via Checkov. Intentional misconfigurations included to validate controls fire. |
| **P02: Kubernetes Baseline** | KIND cluster with Kyverno admission control and Trivy image scanning. Intentional policy violations by design — controls are verified to work, not assumed. |
| **P03: Container Supply Chain** | SBOM generation via Syft, keyless image signing via Cosign/Sigstore, OCI-attached signature stored in GHCR. Tamper-evident provenance end-to-end. |
| **P05: Multi-Gate CI Pipeline** | Four independent jobs: SAST (Semgrep), SCA (pip-audit), secrets detection (Gitleaks), IaC scanning (Checkov). Discrete pass/fail per gate, named artifacts, SARIF output. |
| **P07: Policy as Code** | OPA + Conftest enforcing custom Rego policies as a CI gate. Per-gate job structure, dynamic pipeline summary via `needs.<job>.result`. |
| **P08: Runtime Detection** | Five custom Falco rules firing against live container behaviour. Gate 3 uses Python/PyYAML structural validation. Outbound connection rules scoped to avoid false positives. |

---

## Azure CNAPP Lab

Live hybrid environment: Azure Arc-connected on-premises VM (`siemvm`) alongside Azure-native VM (`Defendervm01`). Defender for Cloud CSPM + CWPP Plan 2, Microsoft Sentinel SIEM, MDE — configured, not just deployed.

---

## Core Tooling

`Azure` `Defender for Cloud` `Microsoft Sentinel` `CrowdStrike Falcon` `Terraform` `Checkov` `GitHub Actions` `Gitleaks` `Semgrep` `Syft` `Cosign` `Kyverno` `Trivy` `Falco` `OPA/Conftest` `Docker` `Kubernetes` `Python` `Linux`

---

## TryHackMe

[![TryHackMe](tryhackme.png)](https://tryhackme.com/p/GooseyintheShell)
