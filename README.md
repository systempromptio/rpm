<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://systemprompt.io/files/images/logo.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://systemprompt.io/files/images/logo-dark.svg">
  <img src="https://systemprompt.io/files/images/logo-dark.svg" alt="systemprompt.io" width="320">
</picture>

# systempromptio/rpm

**DNF/YUM repository for the systemprompt AI governance gateway.**

Served at [`rpm.systemprompt.io`](https://rpm.systemprompt.io). GPG-signed for `x86_64` and `aarch64` on RHEL 9 / Rocky 9 / Fedora 40+.

The governance layer for AI agents — a single compiled Rust binary that authenticates, authorises, rate-limits, logs, and costs every AI interaction. Self-hosted, air-gap capable, provider-agnostic.

[**systemprompt.io**](https://systemprompt.io) · [**Documentation**](https://systemprompt.io/documentation/) · [**Main repo**](https://github.com/systempromptio/systemprompt-template) · [**Discord**](https://discord.gg/wkAbSuPWpr)

[![Template · MIT](https://img.shields.io/badge/template-MIT-16a34a?style=flat-square)](https://github.com/systempromptio/systemprompt-template/blob/main/LICENSE)
[![Core · BSL--1.1](https://img.shields.io/badge/core-BSL--1.1-2b6cb0?style=flat-square)](https://github.com/systempromptio/systemprompt-core/blob/main/LICENSE)

</div>

---

## Install

```bash
sudo curl -fsSL -o /etc/yum.repos.d/systemprompt.repo \
  https://rpm.systemprompt.io/systemprompt.repo

sudo rpm --import https://rpm.systemprompt.io/gpg.key
sudo dnf install systemprompt
```

Full configuration + systemd setup: [systemprompt-template/docs/install/rpm.md](https://github.com/systempromptio/systemprompt-template/blob/main/docs/install/rpm.md).

## Supported distributions

- RHEL 9
- Rocky Linux 9
- AlmaLinux 9
- Fedora 40+
- Amazon Linux 2023

## Architectures

- `x86_64`
- `aarch64`

## Licence

Packaging: MIT (this repo). Compiled binary: `MIT AND BUSL-1.1` — template code is [MIT](https://github.com/systempromptio/systemprompt-template/blob/main/LICENSE); the compiled binary links `systemprompt-core` which is [BSL-1.1](https://github.com/systempromptio/systemprompt-core/blob/main/LICENSE).
