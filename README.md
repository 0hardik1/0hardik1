# Hi, I'm Hardik 👋

I do platform security: securing the cloud and compute foundations every product team builds on, so the safe path is the default path.

At Block, I secure the platform shared by Square, Cash App, and Afterpay: multi-tenant Kubernetes (60+ clusters, thousands of services) on an AWS organization of roughly 10,000 accounts. The work spans three layers:

- **Cloud security.** Foundational AWS controls at organization scale: service control policies (SCPs) and resource control policies (RCPs), data perimeters, permission boundaries, Golden-AMI enforcement across ~10,000 accounts, IAM-authenticated service networking for Block's AWS VPC Lattice adoption, and least-privilege IAM reduction driven by real usage data.
- **Compute security.** Kubernetes admission control (OPA/Rego), container image signature and build-attestation verification with Sigstore/Cosign across all Block Kubernetes platforms, workload isolation with gVisor, and hardening the Terraform CI/CD pipelines that deploy our infrastructure. Earlier: the security roadmap for Twitter's ~200k-node Kubernetes migration, and Twitter's Kubernetes Security Standard.
- **Securing AI agents.** Agentic workloads are the newest untrusted tenant on every platform. Some of the open-source work below is about giving them isolation and least-privilege paths.

Underneath: a decade of threat modeling and security design review at Block, Twitter, Salesforce, and Synopsys.

---

## Open Source

Recent platform-security work across cloud, compute, and AI-agent security:

- **[kubesplaining](https://github.com/0hardik1/kubesplaining)** [![stars](https://img.shields.io/github/stars/0hardik1/kubesplaining?style=social)](https://github.com/0hardik1/kubesplaining) Kubernetes security assessment CLI that maps multi-hop RBAC privilege-escalation paths to cluster takeover.
- **[awsmux](https://github.com/0hardik1/awsmux)** [![stars](https://img.shields.io/github/stars/0hardik1/awsmux?style=social)](https://github.com/0hardik1/awsmux) CLI that runs one AWS command across hundreds of accounts in parallel, with a built-in MCP server for AI agents.
- **[rbac-why-can-i](https://github.com/0hardik1/rbac-why-can-i)** [![stars](https://img.shields.io/github/stars/0hardik1/rbac-why-can-i?style=social)](https://github.com/0hardik1/rbac-why-can-i) `kubectl` plugin that traces *why* an RBAC permission is granted, showing the exact Role/Binding chain.
- **[agentmoat](https://github.com/0hardik1/agentmoat)**: moves Kubernetes workloads from runc to gVisor to blunt container-escape, safely and reversibly.
- **[eks-identity-migrator](https://github.com/0hardik1/eks-identity-migrator)**: audits IRSA usage and migrates EKS clusters to Pod Identity with verification and rollback.
- **[eks-scp](https://github.com/0hardik1/eks-scp)**: highest-impact AWS Organizations SCPs for EKS, built on the EKS IAM condition keys.

---

## Writing

- [Kube-Policies: Guardrails for Apps Running in Kubernetes](https://developer.squareup.com/blog/kube-policies-guardrails-for-apps-running-in-kubernetes/)
- [Kube-Policies BinauthZ: Closing the Supply Chain Gap in Kubernetes](https://engineering.block.xyz/blog/kube-policies-binauthz-closing-the-supply-chain-gap-in-kubernetes)

---

## Credentials

OSCP &nbsp;|&nbsp; Advanced Cloud Security Practitioner (CSA) &nbsp;|&nbsp; M.S. Cyber Security, NYU

---

## Stack

Go &nbsp;|&nbsp; Python &nbsp;|&nbsp; Rego &nbsp;|&nbsp; Terraform &nbsp;|&nbsp; Kubernetes &nbsp;|&nbsp; AWS &nbsp;|&nbsp; OPA/Gatekeeper
