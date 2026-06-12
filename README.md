<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=210&color=0:020617,45:111827,100:2563EB&text=m2hcz&fontColor=F8FAFC&fontSize=54&fontAlignY=38&desc=Offensive%20Security%20%C2%B7%20Vulnerability%20Research%20%C2%B7%20Red%20Team&descAlignY=58&descSize=16" alt="m2hcz banner" />

<img src="https://github.com/m2hcz.png" alt="m2hcz avatar" width="104" height="104" />

<br/>

<a href="mailto:m2hczs@proton.me">
  <img src="https://img.shields.io/badge/Email-m2hczs@proton.me-111827?style=for-the-badge&logo=protonmail&logoColor=8B5CF6" alt="email" />
</a>
<a href="https://x.com/inf0secc">
  <img src="https://img.shields.io/badge/X-@inf0secc-111827?style=for-the-badge&logo=x&logoColor=white" alt="x" />
</a>
<a href="https://github.com/m2hcz">
  <img src="https://img.shields.io/badge/GitHub-m2hcz-111827?style=for-the-badge&logo=github&logoColor=white" alt="github" />
</a>

<br/><br/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=2600&pause=800&color=60A5FA&center=true&vCenter=true&width=760&lines=I+break+systems+to+make+them+harder+to+break.;Web%2C+cloud%2C+identity%2C+CI%2FCD%2C+and+local-app+attack+surfaces.;Reproducible+PoCs.+Clear+impact.+Practical+fixes." alt="typing animation" />

</div>

---

## About

I work on offensive security with a focus on **vulnerability research, exploitability validation, and practical remediation**.

My work is centered on one question:

> As an attacker, what can I actually do, and how do we prove it safely?

I care about impact, not noise. A good finding is reproducible, scoped, clearly explained, and useful to the engineers who need to fix it.

---

## Current Focus `2026`

```text
> Web application vulnerability research
> OAuth / callback / session binding flaws
> CSRF and local-app request forgery
> Cloud IAM and workload identity abuse
> CI/CD, GitHub Actions, and supply-chain attack paths
> AI developer tooling security and agent-assisted review workflows
> Bug bounty triage discipline: impact, exploitability, reproducibility
```

---

## Research Areas

<table>
  <tr>
    <td width="50%">
      <h3>Web & AppSec</h3>
      <p>Auth bypass, IDOR, access-control failures, XSS with real impact, CSRF, request smuggling, SSRF, file upload abuse, and business-logic flaws.</p>
    </td>
    <td width="50%">
      <h3>Identity & Cloud</h3>
      <p>OAuth/OIDC edge cases, token exchange, metadata pivots, IAM misconfiguration chains, workload identity boundaries, and secret exposure paths.</p>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3>Supply Chain</h3>
      <p>Dependency confusion, package trust, CI runner isolation, artifact poisoning, build cache leaks, and GitHub Actions hardening.</p>
    </td>
    <td width="50%">
      <h3>Exploit Validation</h3>
      <p>Safe PoCs, controlled test environments, fake backends, local reproduction, scanner triage, and evidence that survives security review.</p>
    </td>
  </tr>
</table>

---

## Toolbelt

<div align="center">

### Languages

<img src="https://skillicons.dev/icons?i=python,go,rust,c,bash,ts,js,lua" alt="languages" />

### Infra & Platforms

<img src="https://skillicons.dev/icons?i=linux,docker,kubernetes,terraform,aws,gcp,azure,cloudflare,githubactions" alt="infra" />

### Security Workflow

<img src="https://img.shields.io/badge/Burp_Suite-111827?style=for-the-badge&logo=burpsuite&logoColor=FF6633" alt="burp suite" />
<img src="https://img.shields.io/badge/mitmproxy-111827?style=for-the-badge&logo=mitmproxy&logoColor=white" alt="mitmproxy" />
<img src="https://img.shields.io/badge/Frida-111827?style=for-the-badge&logo=frida&logoColor=white" alt="frida" />
<img src="https://img.shields.io/badge/Ghidra-111827?style=for-the-badge&logoColor=white" alt="ghidra" />
<img src="https://img.shields.io/badge/Semgrep-111827?style=for-the-badge&logo=semgrep&logoColor=00C4B3" alt="semgrep" />
<img src="https://img.shields.io/badge/gosec-111827?style=for-the-badge&logo=go&logoColor=00ADD8" alt="gosec" />
<img src="https://img.shields.io/badge/Nuclei-111827?style=for-the-badge&logoColor=white" alt="nuclei" />
<img src="https://img.shields.io/badge/Playwright-111827?style=for-the-badge&logo=playwright&logoColor=45BA4B" alt="playwright" />

</div>

---

## How I Work

```text
1. Scope first
   I keep testing inside explicit authorization and defined boundaries.

2. Reproduce before reporting
   I separate scanner output from exploitable behavior.

3. Prove impact safely
   I prefer controlled PoCs, local fake services, and non-destructive payloads.

4. Write for engineers
   Reports include affected paths, attack preconditions, reproduction steps,
   impact, and practical remediation.

5. Reduce noise
   If it cannot answer "as an attacker I could...", it is not ready.
```

---

## Selected Workflows

<details>
<summary><b>Bug bounty / disclosure workflow</b></summary>

```text
Recon -> scope check -> candidate finding -> exploitability validation
      -> impact calibration -> report drafting -> triage response
      -> remediation notes -> retest if requested
```

</details>

<details>
<summary><b>Repository security review workflow</b></summary>

```text
Threat model -> source/sink mapping -> auth boundary review
             -> local dynamic validation -> scanner triage
             -> minimal PoC -> report-ready evidence
```

</details>

<details>
<summary><b>Current research notes</b></summary>

```text
Local developer tooling:
  - localhost service trust boundaries
  - CSRF against local management UIs
  - token forwarding from local apps to cloud APIs

Identity flows:
  - missing state/nonce binding
  - account/session fixation
  - callback trust and redirect handling

AI security:
  - AI connector trust boundaries
  - review payload exposure
  - agent workflow abuse
```

</details>

---

## GitHub Activity

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=m2hcz&show_icons=true&theme=github_dark&hide_border=true&bg_color=00000000&rank_icon=github&include_all_commits=true" alt="github stats" />
<img height="165" src="https://streak-stats.demolab.com?user=m2hcz&theme=github-dark-blue&hide_border=true&background=00000000" alt="github streak" />

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=m2hcz&theme=github-compact&hide_border=true&bg_color=00000000&line=60A5FA&point=FFFFFF&area=true&area_color=1E40AF" alt="activity graph" />

<br/>

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=m2hcz&theme=github_dark" alt="profile summary" />

</div>

---

## Contact

The best way to reach me is email:

```text
m2hczs@proton.me
```

For security reports, include scope, affected asset, reproduction steps, impact, and remediation context.

<div align="center">

<sub>Responsible disclosure · Authorized testing only · Evidence over noise</sub>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&height=120&section=footer&color=0:2563EB,45:111827,100:020617" alt="footer" />

</div>
