![Open Society banner](banner.png?v=2)

# Open Society

We build open-source network analysis and monitoring tools in Dart and Flutter —
one cross-platform app and the libraries that power it.

[![Stars](https://img.shields.io/github/stars/osociety?style=for-the-badge&label=stars&color=A06BFF)](https://github.com/osociety)
[![Followers](https://img.shields.io/github/followers/osociety?style=for-the-badge&label=followers&color=6630A5&logo=github&logoColor=white)](https://github.com/osociety)
[![Sponsoring](https://img.shields.io/liberapay/receives/opensociety?style=for-the-badge&label=sponsoring&color=410E76&logo=liberapay&logoColor=white)](https://liberapay.com/OpenSociety/donate)

---

## Projects

### [Vernet](https://github.com/osociety/vernet)

[![Release](https://img.shields.io/github/v/release/osociety/vernet?style=flat&label=release&color=A06BFF)](https://github.com/osociety/vernet/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/osociety/vernet/total?style=flat&label=downloads&color=6630A5)](https://github.com/osociety/vernet/releases)
[![Stars](https://img.shields.io/github/stars/osociety/vernet?style=flat&label=stars&color=6630A5)](https://github.com/osociety/vernet)
[![Apache-2.0](https://img.shields.io/github/license/osociety/vernet?style=flat&label=license&color=6630A5)](https://github.com/osociety/vernet/blob/main/LICENSE)

Know your network. Vernet finds the devices and services reachable on your local
network, pings hosts, scans ports, resolves names in both directions, and
measures your connection — with per-device history and security findings.

**Get it** — [Google Play](https://play.google.com/store/apps/details?id=org.fsociety.vernet.store)
· [F-Droid](https://f-droid.org/packages/org.fsociety.vernet)
· [Microsoft Store](https://apps.microsoft.com/detail/9N1170N3PHMM)
· [Snap](https://snapcraft.io/vernet)
· [macOS and Linux archives](https://github.com/osociety/vernet/releases/latest)

iOS builds are not released yet.

### [Network Tools](https://github.com/osociety/network_tools)

[![pub](https://img.shields.io/pub/v/network_tools?style=flat&label=pub&color=A06BFF)](https://pub.dev/packages/network_tools)
[![BSD-3-Clause](https://img.shields.io/github/license/osociety/network_tools?style=flat&label=license&color=6630A5)](https://github.com/osociety/network_tools/blob/main/LICENSE)

The engine underneath Vernet, and usable on its own: a pure Dart library for
host discovery, port scanning, mDNS, ping, and DNS lookups on Android, iOS,
Linux, macOS, Windows, and the web.

### [Network Tools Flutter](https://github.com/osociety/network_tools_flutter)

[![pub](https://img.shields.io/pub/v/network_tools_flutter?style=flat&label=pub&color=A06BFF)](https://pub.dev/packages/network_tools_flutter)
[![Apache-2.0](https://img.shields.io/github/license/osociety/network_tools_flutter?style=flat&label=license&color=6630A5)](https://github.com/osociety/network_tools_flutter/blob/main/LICENSE)

The Flutter layer on top of `network_tools`, where it absorbs the platform
limitations the pure Dart package cannot reach — mDNS permissions, background
scans, and the differences between mobile and desktop network stacks.

---

## Get involved

| Where | What goes there |
| :--- | :--- |
| [Discussions](https://github.com/osociety/vernet/discussions) | Release announcements, Q&A, feature ideas, polls |
| [Issues](https://github.com/osociety/vernet/issues) | Bugs and platform-specific problems |
| [Contribute](https://github.com/osociety/.github/blob/main/CONTRIBUTING.md) | How to build, test, and send a change for review |
| [Report a vulnerability](https://github.com/osociety/.github/blob/main/SECURITY.md) | Private disclosure, not a public issue |
| [Code of conduct](https://github.com/osociety/.github/blob/main/CODE_OF_CONDUCT.md) | What we expect of each other |

Beta builds are where most of the real testing happens. They are announced in
[Discussions](https://github.com/osociety/vernet/discussions/categories/announcements)
before each release and need nothing but a device you already own.

## Support

1. **Star the repositories** — it is the cheapest way to help them get found.
2. **Rate Vernet** on [Google Play](https://play.google.com/store/apps/details?id=org.fsociety.vernet.store) or the [Microsoft Store](https://apps.microsoft.com/detail/9N1170N3PHMM).
3. **Fund the work** — [Liberapay](https://liberapay.com/OpenSociety/donate),
   [GitHub Sponsors](https://github.com/sponsors/fs0c13ty), or
   [Ko-fi](https://ko-fi.com/fs0c13ty).

## Policies

[Privacy Policy](PRIVACY_POLICY.md) · [Terms of Service](TERMS_OF_SERVICE.md) ·
[No Refund Policy](NO_REFUND_POLICY.md)
