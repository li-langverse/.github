# li-langverse

**Li** is a secure-by-design language and runtime for systems software, scientific computing, and agentic infrastructure. This organization hosts the compiler, web server, package ecosystem, and related tooling.

## Main repositories

| Repo | Description |
|------|-------------|
| [**lic**](https://github.com/li-langverse/lic) | Li compiler, runtime, and standard library |
| [**li-httpd**](https://github.com/li-langverse/li-httpd) | High-performance HTTP edge server (TOML-configured) |
| [**lis**](https://github.com/li-langverse/lis) | Li webserver — secure definitions in `.toml` |
| [**lip**](https://github.com/li-langverse/lip) | Li package manager |
| [**roadmap**](https://github.com/li-langverse/roadmap) | Ecosystem governance and agent-kit |

## Development source: GitLab

**GitHub is the public mirror.** Day-to-day development happens on our homelab GitLab instance; a mirror syncs selected projects here every ~15 minutes.

| Resource | URL |
|----------|-----|
| Sign in | https://gitlab.lilangverse.xyz/users/sign_in |
| Explore (public projects) | https://gitlab.lilangverse.xyz/explore |
| **li-langverse** group | https://gitlab.lilangverse.xyz/li-langverse |
| Example projects | [lic](https://gitlab.lilangverse.xyz/li-langverse/lic) · [lis](https://gitlab.lilangverse.xyz/li-langverse/lis) · [li-cursor-agents](https://gitlab.lilangverse.xyz/li-langverse/li-cursor-agents) |
| Container registry | https://registry.gitlab.lilangverse.xyz |
| Health | https://gitlab.lilangverse.xyz/-/health |

### Public vs private

Projects in the **li-langverse** group are currently **private** — you must sign in to browse or clone. To allow anonymous access:

1. Open the project on GitLab → **Settings** → **General**
2. Expand **Visibility, project features, permissions**
3. Set **Project visibility** to **Public** → **Save changes**

After that, the project appears on [Explore](https://gitlab.lilangverse.xyz/explore) and can be cloned without login.

### WAN access

From the public internet, **gitlab.lilangverse.xyz** resolves via DNS:

```
gitlab.lilangverse.xyz  →  77.23.124.82
```

HTTPS is terminated at the homelab edge (li-httpd on blackpearl). Ensure ports **80** and **443** reach that host.

On LAN, you can also use `*.homelab.lan` hostnames or a hosts-file entry pointing at the edge node.

## Contributing

- **Issues & PRs on GitHub** — welcome on mirrored repos; changes are synced back to GitLab when configured.
- **Primary workflow** — branch on GitLab, merge there; mirror propagates to GitHub.
