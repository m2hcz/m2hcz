<div align="center">

<img src="https://capsule-render.vercel.app/api?type=rect&height=190&color=0:000000,55:090909,100:161616&text=m2hcz&fontColor=FFFFFF&fontSize=62&fontAlignY=42&desc=Offensive%20Security%20%C2%B7%20AppSec%20%C2%B7%20Vulnerability%20Research%20%C2%B7%20Backend%20Engineering&descAlignY=67&descSize=15" alt="m2hcz banner" />

<br/>

<a href="mailto:m2hczs@proton.me">
  <img src="https://img.shields.io/badge/Email-m2hczs%40proton.me-000000?style=for-the-badge&logo=protonmail&logoColor=white" alt="Email" />
</a>
<a href="https://x.com/inf0secc">
  <img src="https://img.shields.io/badge/X-%40inf0secc-000000?style=for-the-badge&logo=x&logoColor=white" alt="X" />
</a>
<a href="https://github.com/m2hcz">
  <img src="https://img.shields.io/badge/GitHub-m2hcz-000000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
</a>

<br/><br/>

<sub>
Senior Software Engineer and Offensive Security Researcher focused on authorization, trust boundaries,
secure backend architecture, reproducible exploitation, and practical remediation.
</sub>

</div>

---

## Profile

I work at the intersection of **offensive security, application security, and production software engineering**.

My background in backend architecture, distributed systems, server-authoritative design, performance, and abuse resistance directly informs how I approach security research. I do not treat a scanner result as a vulnerability. A finding is only complete when it is:

- reproducible;
- technically scoped;
- tied to a credible attack path;
- supported by controlled evidence;
- understandable by the engineers responsible for fixing it.

My objective is not to maximize the number of findings. It is to identify the weaknesses that matter, prove them safely, and help teams ship durable fixes.

<table>
<tr>
<td><strong>12+ years</strong><br/><sub>software engineering</sub></td>
<td><strong>9+ years</strong><br/><sub>information security</sub></td>
<td><strong>2 assigned CVEs</strong><br/><sub>public vulnerability research</sub></td>
<td><strong>Remote · UTC-3</strong><br/><sub>Brazil</sub></td>
</tr>
</table>

---

## Selected Security Research

### CVE-2026-54094 — File Browser

**Symlink-based directory scope bypass**

File Browser enforced per-user directory scope against lexical traversal, but affected handlers followed symbolic links before file access. This allowed scoped users — and, in some public-share scenarios, unauthenticated recipients — to interact with files outside the directory boundary the application was expected to enforce.

**Impact:** out-of-scope file read, overwrite, and sharing  
**Classes:** CWE-22 · CWE-59  
**Severity:** High · CVSS 7.5  
**Status:** fixed in `v2.63.14`

[GitHub Advisory](https://github.com/filebrowser/filebrowser/security/advisories/GHSA-239w-m3h6-ch8v) ·
[CVE Record](https://www.cve.org/CVERecord?id=CVE-2026-54094) ·
[Fixed Release](https://github.com/filebrowser/filebrowser/releases/tag/v2.63.14) ·
[Patch](https://github.com/filebrowser/filebrowser/commit/7c2c0a11b31b2bb214d741005a0b02b1764208b3)

---

### CVE-2026-28740 — Gitea

**Git LFS cross-repository authorization bypass**

An authorization flaw in Gitea's cross-repository Git LFS flow allowed a user without sufficient source-repository permissions to authorize and retrieve private LFS objects belonging to another repository.

**Impact:** unauthorized access to private Git LFS objects  
**Classes:** CWE-639 · CWE-863  
**Severity:** High · CVSS 7.1  
**Status:** fixed through `PR #38006`

[CVE Record](https://www.cve.org/CVERecord?id=CVE-2026-28740) ·
[Fix PR](https://github.com/go-gitea/gitea/pull/38006) ·
[Security Release](https://blog.gitea.com/release-of-1.26.3-and-1.26.4/)

---

### GitHub CLI

**Symlink path traversal and Git hook injection in `gh run download`**

A path-boundary weakness allowed writes outside the intended download directory and could be used to plant an executable Git hook.

**Impact:** arbitrary out-of-boundary write with code-execution implications  
**Classes:** CWE-22 · CWE-59  
**Status:** reported through HackerOne and validated by GitHub Security  
**Reference:** HackerOne report `#3786623`

---

### Additional Research and Responsible Disclosure

Research or security reports have also involved:

`Gemini CLI` · `NASA VDP` · `Tesla` · `xAI / X` · `Discord` · `Automattic / WordPress.com` · `USP` · `Gov.br` · `Roblox`

These names identify the relevant program, product, or ecosystem. They do not imply employment, endorsement, or a commercial relationship.

---

## Current Research Areas

| Area | What I examine |
|---|---|
| **Authorization** | object-level access control, cross-tenant access, scope enforcement, confused-deputy behavior |
| **Identity and sessions** | OAuth/OIDC callback binding, state and nonce handling, fixation, account linking, trust transitions |
| **Web and API security** | SSRF, IDOR, CSRF, request smuggling, unsafe file handling, business-logic abuse |
| **CI/CD and supply chain** | runner isolation, artifact trust, cache poisoning, workflow permissions, dependency boundaries |
| **Cloud and IAM** | workload identity, metadata-service access, role chaining, exposed secrets, policy misconfiguration |
| **AI-assisted systems** | connector trust, agent permissions, prompt-to-action boundaries, review and tool-execution flows |
| **Secure backend design** | server-authoritative validation, anti-abuse controls, concurrency, persistence, integrity |

---

## Methodology

```text
authorization
    ↓
attack-surface mapping
    ↓
candidate weakness
    ↓
local or controlled reproduction
    ↓
exploitability validation
    ↓
impact calibration
    ↓
engineer-ready report
    ↓
remediation review and retest
```

The process is governed by three constraints:

1. **Scope is absolute.** Testing remains inside explicit authorization.
2. **Evidence precedes severity.** Scanner output is a lead, not a conclusion.
3. **Impact is proven without causing operational harm.** PoCs are controlled, minimal, and non-destructive.

<details>
<summary><strong>External disclosure workflow</strong></summary>

<br/>

```text
scope review
→ reconnaissance
→ attack hypothesis
→ safe validation
→ impact analysis
→ disclosure
→ triage support
→ retest
```

</details>

<details>
<summary><strong>Repository and architecture review workflow</strong></summary>

<br/>

```text
threat model
→ trust-boundary mapping
→ source-to-sink analysis
→ authorization review
→ dynamic validation
→ minimal PoC
→ remediation guidance
```

</details>

---

## Engineering Background

Security research is stronger when it is backed by an understanding of how production systems are designed, deployed, and operated.

My engineering work includes:

- secure backend architecture;
- distributed and concurrent systems;
- real-time client-server networking;
- server-authoritative validation;
- anti-cheat and abuse resistance;
- persistence, sharding, and data integrity;
- performance analysis and optimization;
- CI/CD, infrastructure, and operational reliability;
- secure code review and remediation design.

### Languages

`Python` · `TypeScript` · `JavaScript` · `Go` · `Rust` · `C` · `C#` · `Lua / Luau` · `Bash` · `SQL`

### Platforms and Infrastructure

`Linux` · `Docker` · `Kubernetes` · `Terraform` · `Cloudflare` · `GitHub Actions` · `Nginx` · `PostgreSQL` · `Redis`

### Security Tooling

`Burp Suite` · `mitmproxy` · `Frida` · `Ghidra` · `Radare2` · `pwntools` · `Z3` · `Semgrep` · `Nuclei` · `Nmap` · `Wireshark` · `Playwright`

---

## Selected Open-Source Work

| Project | Purpose | Stack |
|---|---|---|
| [`pathward`](https://github.com/m2hcz/pathward) | defensive path-handling library against traversal, symlink escape, Zip Slip, and TOCTOU | Python |
| [`ReconMapper v2`](https://github.com/m2hcz/reconmapper-v2.0) | repeatable reconnaissance and attack-surface mapping | Python |
| [`SQLi Scanner`](https://github.com/m2hcz/Sqli-Automaticly-Scanner) | automated SQL injection discovery and payload validation | TypeScript |
| [`Next.js Middleware PoC`](https://github.com/m2hcz/PoC-for-Next.js-Middleware) | research into framework-level authorization boundaries | JavaScript |
| [`NetSentinel`](https://github.com/m2hcz/NetSentinel-1.0) | network monitoring and threat-detection framework | Luau |
| [`PhantomNet`](https://github.com/m2hcz/PhantomNet) | optimized client-server networking and compact synchronization | Luau |

---

## Working Principles

> **Security research should reduce uncertainty.**

That means:

- no severity inflation;
- no unverifiable impact claims;
- no destructive proof of concept;
- no ambiguity between observation and exploitation;
- no remediation advice disconnected from the real architecture.

Reports are written for the people who must reproduce, prioritize, fix, and verify the issue.

---

## GitHub Activity

<details>
<summary><strong>View statistics</strong></summary>

<br/>

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=m2hcz&show_icons=true&theme=github_dark&hide_border=true&bg_color=00000000&title_color=FFFFFF&icon_color=B8B8B8&text_color=C9D1D9&rank_icon=github&include_all_commits=true" alt="GitHub statistics" />

<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=m2hcz&layout=compact&theme=github_dark&hide_border=true&bg_color=00000000&title_color=FFFFFF&text_color=C9D1D9&langs_count=8" alt="Most used languages" />

<br/>

<img height="165" src="https://streak-stats.demolab.com?user=m2hcz&theme=github-dark-blue&hide_border=true&background=00000000&ring=FFFFFF&fire=B8B8B8&currStreakLabel=FFFFFF" alt="GitHub contribution streak" />

</div>

</details>

---

## Contact

For engineering, AppSec, offensive security, or focused vulnerability-research work:

**Email:** [m2hczs@proton.me](mailto:m2hczs@proton.me)  
**GitHub:** [github.com/m2hcz](https://github.com/m2hcz)  
**X:** [@inf0secc](https://x.com/inf0secc)

For security reports, include:

```text
scope
affected asset
preconditions
reproduction steps
observed impact
supporting evidence
remediation context
```

<div align="center">

<br/>

<img src="https://img.shields.io/badge/Responsible_Disclosure-000000?style=flat-square&labelColor=000000&color=242424" alt="Responsible disclosure" />
<img src="https://img.shields.io/badge/Authorized_Testing_Only-000000?style=flat-square&labelColor=000000&color=242424" alt="Authorized testing only" />
<img src="https://img.shields.io/badge/Evidence_Over_Noise-000000?style=flat-square&labelColor=000000&color=242424" alt="Evidence over noise" />

<br/><br/>

<sub>Build secure systems. Verify assumptions. Report what matters.</sub>

</div>

<img src="https://capsule-render.vercel.app/api?type=rect&height=70&section=footer&color=0:000000,50:090909,100:161616" alt="footer" />
