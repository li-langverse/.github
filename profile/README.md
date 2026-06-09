# li-langverse

**Li** is an open ecosystem for high-performance computing, scientific computing, and AI — with a native compiler (`lic`), package manager (`lip`), secure web server (`lis` / `li-httpd`), and provable builds.

This GitHub organization is a **read-only mirror** of our primary development on GitLab. Clone, branch, and merge on GitLab; GitHub updates automatically.

---

## Browse source on GitLab (no account needed for public projects)

Public projects can be read without signing in.

| What | URL |
|------|-----|
| **Explore all public projects** | https://gitlab.lilangverse.xyz/explore |
| **Group home** | https://gitlab.lilangverse.xyz/li-langverse |
| **Example project** | https://gitlab.lilangverse.xyz/li-langverse/lic |

**Clone a public repo:**

```bash
git clone https://gitlab.lilangverse.xyz/li-langverse/lic.git
```

**Browse in the UI:** open any public project → **Repository** → files, commits, and tags are visible without login. Issues and merge requests on public projects are also readable.

If a project shows **404** or asks you to sign in, it is **private** — request access from a maintainer or wait until visibility is changed to public.

---

## Main repositories

| Repo | Role | GitLab | GitHub mirror |
|------|------|--------|---------------|
| **lic** | Li compiler, stdlib, libernetes | [GitLab](https://gitlab.lilangverse.xyz/li-langverse/lic) | [GitHub](https://github.com/li-langverse/lic) |
| **lis** | Secure Li web server (li-httpd) | [GitLab](https://gitlab.lilangverse.xyz/li-langverse/lis) | [GitHub](https://github.com/li-langverse/lis) |
| **li-httpd** | Li HTTP daemon package | [GitLab](https://gitlab.lilangverse.xyz/li-langverse/li-httpd) | [GitHub](https://github.com/li-langverse/li-httpd) |
| **lip** | Package manager | [GitLab](https://gitlab.lilangverse.xyz/li-langverse/lip) | [GitHub](https://github.com/li-langverse/lip) |
| **lit** | Testing library | [GitLab](https://gitlab.lilangverse.xyz/li-langverse/lit) | [GitHub](https://github.com/li-langverse/lit) |
| **roadmap** | Ecosystem governance & agent-kit | [GitLab](https://gitlab.lilangverse.xyz/li-langverse/roadmap) | [GitHub](https://github.com/li-langverse/roadmap) |
| **benchmarks** | Perf dashboard data | [GitLab](https://gitlab.lilangverse.xyz/li-langverse/benchmarks) | [GitHub](https://github.com/li-langverse/benchmarks) |
| **lib** | Agentic browser packages | [GitLab](https://gitlab.lilangverse.xyz/li-langverse/lib) | [GitHub](https://github.com/li-langverse/lib) |

**Live docs (GitHub Pages):**

- [Benchmarks dashboard](https://li-langverse.github.io/benchmarks/)
- [Development overview](https://li-langverse.github.io/roadmap/development-overview/)
- [Master plan (PH tracker)](https://github.com/li-langverse/lic/blob/main/docs/superpowers/plans/2026-05-14-li-master-plan.md)
- [Getting started (tools)](https://github.com/li-langverse/lic/blob/main/docs/guide/getting-started-tools.md)

**Container images:** `ghcr.io/li-langverse/*` (GitHub Container Registry).

---

## Homelab hosting (`*.lilangverse.xyz`)

Services run on a homelab Kubernetes cluster (engine node) and are exposed at the edge via **li-httpd**.

| Host | Purpose | WAN DNS |
|------|---------|---------|
| `gitlab.lilangverse.xyz` | **Primary git** — develop here | `A` → `77.23.124.82` |
| `lip.lilangverse.xyz` | Li package registry API | `A` → `77.23.124.82` |

**Policy:** GitLab is primary for git and CI. GitHub mirrors repos every ~15 minutes. Do not push commits directly to `github.com/li-langverse/*` for day-to-day development.

**LAN:** cluster services use in-cluster DNS (e.g. `gitlab.gitlab.svc`). **WAN:** public hostnames above resolve to the Fritz-box WAN IP and terminate TLS at the edge (ports **80** / **443**).

---

## Make a GitLab project public

Maintainers only (project **Owner** or **Maintainer**):

1. Open the project on GitLab → **Settings** → **General**.
2. Expand **Visibility, project features, permissions**.
3. Set **Project visibility** to **Public**.
4. Save changes.

The project then appears on https://gitlab.lilangverse.xyz/explore and is readable without login. The GitLab→GitHub mirror will continue to sync; ensure the matching GitHub repo visibility matches your intent.

To create a new **public** project: **New project** → set visibility to **Public** at creation time, under the `li-langverse` group.

---

## Contributing

1. Browse or clone from **GitLab** (links above).
2. Read [roadmap engineering standards](https://github.com/li-langverse/roadmap/blob/main/docs/ecosystem/engineering-standards.md).
3. Open a **merge request** on GitLab (feature branch → `main`).

Questions and governance: [li-langverse/roadmap](https://gitlab.lilangverse.xyz/li-langverse/roadmap).
