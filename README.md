<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=200&color=0:020617,40:111827,100:2563EB&text=m2hcz&fontColor=F8FAFC&fontSize=54&fontAlignY=38&desc=Offensive%20Security%20Research%20%C2%B7%20Exploit%20Validation%20%C2%B7%20Red%20Team&descAlignY=58&descSize=14&descAlignX=50" alt="m2hcz banner" />

<a href="https://github.com/m2hcz">
  <img src="https://github.com/m2hcz.png" alt="m2hcz avatar" width="112" height="112" style="border-radius:50%;" />
</a>

<br/><br/>

<a href="mailto:m2hczs@proton.me">
  <img src="https://img.shields.io/badge/Email-m2hczs@proton.me-111827?style=for-the-badge&logo=protonmail&logoColor=8B5CF6&labelColor=020617" alt="email" />
</a>
<a href="https://x.com/inf0secc">
  <img src="https://img.shields.io/badge/X-@inf0secc-111827?style=for-the-badge&logo=x&logoColor=white&labelColor=020617" alt="x" />
</a>
<a href="https://github.com/m2hcz">
  <img src="https://img.shields.io/badge/GitHub-m2hcz-111827?style=for-the-badge&logo=github&logoColor=white&labelColor=020617" alt="github" />
</a>

<br/><br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&duration=2800&pause=900&color=60A5FA&center=true&vCenter=true&width=860&lines=OAuth+callback+binding.+CSRF+on+local+apps.+CI%2FCD+trust+paths.;Scanner+output+is+a+hypothesis%2C+not+a+finding.;Reproducible+PoCs.+Clear+impact.+Fixes+that+ship." alt="typing animation" />

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%" />

## `>` About

Offensive security research: finding out what an attacker can actually do, and proving it safely enough that engineers trust the fix.

Scanner output dressed up as a finding doesn't count. A result is only done when it's **reproducible, scoped, and actionable** for the team that has to remediate it.

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%" />

## `>` Focus, 2026

| Area | In practice |
|---|---|
| **Identity & auth** | OAuth/OIDC edge cases, missing state/nonce binding, callback trust, session & account fixation |
| **Web & local apps** | CSRF against local management UIs, IDOR, access-control failures, request smuggling, SSRF |
| **Cloud & IAM** | Workload identity boundaries, IAM misconfiguration chains, metadata-service pivots, secret exposure |
| **Supply chain** | CI/CD runner isolation, GitHub Actions hardening, dependency confusion, artifact/build-cache poisoning |
| **AI tooling** | Connector trust boundaries, agent workflow abuse, review-payload exposure in AI-assisted pipelines |

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%" />

## `>` Toolbelt

<div align="center">

**Languages**
<br/>
<img src="https://skillicons.dev/icons?i=python,go,rust,c,bash,ts,js,lua&theme=dark" alt="languages" />

**Infra & Platforms**
<br/>
<img src="https://skillicons.dev/icons?i=linux,docker,kubernetes,terraform,aws,gcp,azure,cloudflare,githubactions&theme=dark" alt="infra" />

**Workflow**
<br/>
<img src="https://img.shields.io/badge/Burp_Suite-111827?style=for-the-badge&logo=burpsuite&logoColor=FF6633&labelColor=020617" alt="burp suite" />
<img src="https://img.shields.io/badge/mitmproxy-111827?style=for-the-badge&logo=mitmproxy&logoColor=white&labelColor=020617" alt="mitmproxy" />
<img src="https://img.shields.io/badge/Frida-111827?style=for-the-badge&logo=frida&logoColor=white&labelColor=020617" alt="frida" />
<img src="https://img.shields.io/badge/Ghidra-111827?style=for-the-badge&logoColor=white&labelColor=020617" alt="ghidra" />
<img src="https://img.shields.io/badge/Semgrep-111827?style=for-the-badge&logo=semgrep&logoColor=00C4B3&labelColor=020617" alt="semgrep" />
<img src="https://img.shields.io/badge/Nuclei-111827?style=for-the-badge&logoColor=white&labelColor=020617" alt="nuclei" />
<img src="https://img.shields.io/badge/Playwright-111827?style=for-the-badge&logo=playwright&logoColor=45BA4B&labelColor=020617" alt="playwright" />

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%" />

## `>` Methodology

```text
scope check -> recon -> candidate finding -> reproduce locally
            -> validate exploitability -> calibrate impact
            -> report for engineers -> retest on fix
```

Three rules that don't change per engagement:

1. **Scope is a hard boundary**, not a suggestion — testing stays inside explicit authorization.
2. **Reproduce before reporting** — scanner output and exploitable behavior are not the same thing.
3. **Prove impact without causing it** — controlled PoCs, local fake services, non-destructive payloads.

<details>
<summary><b>Two engagement types, side by side</b></summary>

<br/>

**External — bug bounty / disclosure**
`recon → scope check → exploitability validation → impact calibration → report → triage response → retest`

**Internal — repo / architecture review**
`threat model → source–sink mapping → auth boundary review → dynamic validation → minimal PoC → report-ready evidence`

</details>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%" />

## `>` Selected Work

<!-- This section carries more weight than any badge below — swap in 2-4 real advisories, CVEs, or writeups. -->

- `CVE-2026-28740`
- `CVE-2026-54094`

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%" />

## `>` GitHub Activity

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=m2hcz&show_icons=true&theme=github_dark&hide_border=true&bg_color=00000000&title_color=60A5FA&icon_color=2563EB&text_color=C9D1D9&rank_icon=github&include_all_commits=true" alt="github stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=m2hcz&layout=compact&theme=github_dark&hide_border=true&bg_color=00000000&title_color=60A5FA&text_color=C9D1D9&langs_count=8" alt="top languages" />

<br/>

<img height="165" src="https://streak-stats.demolab.com?user=m2hcz&theme=github-dark-blue&hide_border=true&background=00000000&ring=2563EB&fire=60A5FA&currStreakLabel=60A5FA" alt="github streak" />

</div>

<img src="https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/colored.png" width="100%" />

## `>` Contact

```text
m2hczs@proton.me
```

For security reports: **scope, affected asset, reproduction steps, impact, remediation context.** No scope, no read.

<div align="center">

<br/>

<img src="https://img.shields.io/badge/Responsible_Disclosure-111827?style=flat-square&labelColor=020617&color=2563EB" alt="responsible disclosure" />
<img src="https://img.shields.io/badge/Authorized_Testing_Only-111827?style=flat-square&labelColor=020617&color=2563EB" alt="authorized testing only" />
<img src="https://img.shields.io/badge/Evidence_Over_Noise-111827?style=flat-square&labelColor=020617&color=2563EB" alt="evidence over noise" />

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&height=110&section=footer&color=0:2563EB,45:111827,100:020617" alt="footer" />
