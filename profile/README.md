# li-langverse

**Li** is a secure-by-design language and runtime for systems software, scientific computing, and agentic infrastructure. This organization hosts the **lic** compiler, **li-httpd** edge server, **lis** web stack, packages, and related tooling.

## Key repositories

| Repo | Description |
|------|-------------|
| [**lic**](https://github.com/li-langverse/lic) | Li compiler, runtime, and standard library |
| [**li-httpd**](https://github.com/li-langverse/li-httpd) | High-performance HTTP edge server (TOML-configured) |
| [**lis**](https://github.com/li-langverse/lis) | Li webserver — secure definitions in `.toml` |
| [**lib**](https://github.com/li-langverse/lib) | Agentic browser packages (lib-core, lib-chrome, lib-acp, TEL) |
| [**lip**](https://github.com/li-langverse/lip) | Li package manager |
| [**roadmap**](https://github.com/li-langverse/roadmap) | Ecosystem governance and agent-kit |

## Documentation

- [lic docs](https://github.com/li-langverse/lic/tree/main/docs) — language, toolchain, and ecosystem guides
- [Getting started (tools)](https://github.com/li-langverse/lic/blob/main/docs/guide/getting-started-tools.md)
- [lis handbook & plans](https://github.com/li-langverse/lis/tree/main/docs)

## GitLab (dev source)

Day-to-day development runs on our **homelab GitLab CE** instance. **GitHub is the public mirror** for visibility; selected projects sync here on a schedule.

| Resource | URL |
|----------|-----|
| GitLab (sign in) | https://gitlab.lilangverse.xyz |
| Explore (public projects) | https://gitlab.lilangverse.xyz/explore |
| **li-langverse** group | https://gitlab.lilangverse.xyz/li-langverse |

Projects in the group are currently **private** — sign in to browse or clone. To expose a project anonymously: open the project → **Settings** → **General** → **Visibility, project features, permissions** → set **Project visibility** to **Public** → save.

### WAN access

Public DNS for GitLab:

```
gitlab.lilangverse.xyz  →  77.23.124.82
```

HTTPS is terminated at the homelab edge (**li-httpd**). Ensure ports **80** and **443** reach that host.

## Contributing

- **GitLab** — primary branch/merge workflow.
- **GitHub** — issues and PRs welcome on mirrored repos; changes can sync back to GitLab when configured.
