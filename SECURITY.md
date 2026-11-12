# Security Policy

## Reporting a vulnerability

Use **Report a vulnerability** on the security tab of the repository —
[vernet](https://github.com/osociety/vernet/security),
[network_tools](https://github.com/osociety/network_tools/security),
[network_tools_flutter](https://github.com/osociety/network_tools_flutter/security).
That opens a private advisory, so the report is not public and you get a
tracked thread with a fixed version and, if you want it, a credit.

Please do not open a normal issue, discussion, or pull request for a security
problem. Those are public from the first comment.

If the form does not work for you, write to
[fs0c19ty@protonmail.com](mailto:fs0c19ty@protonmail.com). There is no PGP key
published for that address, so do not include secrets, tokens, or private keys
in the message — describe the problem and how to reach the affected surface
instead.

## What is in scope

A report is useful when it describes something like:

- Code execution, privilege escalation, or data exposure caused by our software
  processing untrusted input — a crafted hostname, mDNS record, URL, or file
  downloaded from a release.
- A published package or release artifact that has been tampered with, or a
  signing/packaging flaw that lets a bad build be trusted.
- A leak of user data: telemetry, stored scan results, or credentials that end
  up somewhere they should not.
- A weakness in the release or CI pipeline that lets unsigned code reach users.

## What is not a vulnerability

- **The app discovers devices, open ports, and services on the network it is
  running on.** That is the product. A scanner scanning is not a flaw, and
  neither is the fact that a network which permits such discovery makes it
  possible.
- **Findings that need already-rooted or already-controlled devices**, physical
  access to a machine, or access to a victim's network before the app is run.
- **Missing hardening with no reachable impact** — for example, "the app does
  not sandbox a component" without showing what an attacker gains.
- **Reports about third-party services we do not operate** — app stores,
  speed-test endpoints, or package registries. Send those to the operator.
- **Vulnerabilities in dependencies** are handled through Dependabot alerts.
  If you find one that is not already tracked, a private advisory is welcome.

## What to include

The affected repository and version, the platform and OS, what you did, what
happened, what you expected, and the shortest reproduction you can write. A
failing test or a script beats a paragraph.

## How reports are handled

These projects are maintained by one person in the open, with no security team
and no contractual SLA. What you can expect:

1. An acknowledgement, normally within a few days.
2. A quiet fix when the issue is real and exploitable — a patch release, not a
   public advisory first.
3. Credit in the advisory if you want it, and a note in the changelog.

If there is no reply within two weeks, resend the report or try a second
contact route. Silence is usually a missed notification, not a decision.

## Supported versions

Only the latest released version of each project receives security fixes. Older
releases are left on the download page but are not patched, so upgrade before
reporting — many issues are already fixed.

## Hardening already in place

- Secret scanning and push protection are enabled on every repository.
- Dependabot security updates are enabled on every repository.
- Release artifacts for Vernet are built by CI from tagged commits and published
  to GitHub Releases, Google Play, F-Droid, the Microsoft Store, and the Snap
  Store.
