# Contributing

These are the defaults for every Open Society repository. A repository can add
its own contributing guide next to this one, and that guide wins.

## Start here

- **Report it before you build it.** A bug with the platform, app version, and
  what you expected is worth more than a large pull request nobody agreed to.
  Questions and feature ideas go to
  [Discussions](https://github.com/osociety/vernet/discussions); reproducible
  defects go to [Issues](https://github.com/osociety/vernet/issues).
- **Check what is already in flight** — open pull requests and recent issues —
  so two people do not build the same thing.
- **Public API changes in `network_tools` or `network_tools_flutter` need an
  issue first.** Both are published to pub.dev and other projects build on them,
  so a breaking change is a discussion, not a surprise in a release.

## Setting up

| Repository | What it is | Toolchain |
| :--- | :--- | :--- |
| [vernet](https://github.com/osociety/vernet) | Flutter app | Flutter stable, Dart 3.10+ |
| [network_tools](https://github.com/osociety/network_tools) | Pure Dart package | Dart 3.10+ |
| [network_tools_flutter](https://github.com/osociety/network_tools_flutter) | Flutter layer over `network_tools` | Flutter 3.38+, Dart 3.10+ |

```bash
dart pub get        # network_tools
flutter pub get     # vernet, network_tools_flutter
```

Vernet generates part of its source (drift tables, freezed models, get_it
registrations). After changing those inputs:

```bash
dart run build_runner build --delete-conflicting-outputs
```

## Checks to run before pushing

Pure Dart package:

```bash
dart format --output=none --set-exit-if-changed .
dart analyze --fatal-infos
dart test
```

App and Flutter packages:

```bash
dart format --set-exit-if-changed .
flutter analyze --no-fatal-infos --fatal-warnings
flutter test
```

CI runs the same commands on Linux, macOS, and Windows. A pull request that
fails them is not waiting on a review — fix the run first.

## Making the change

- One idea per pull request. A scan-range fix and a settings-screen refactor
  are two pull requests.
- Match the style already in the file rather than introducing a new one.
- Do not hand-edit generated files (`*.g.dart`, `*.freezed.dart`); regenerate
  them.
- A bug fix needs a test that fails before the change and passes after it.
- If you change a public API, update the example, the README, and the
  `CHANGELOG.md` in the same pull request.

## Pull requests

Fill in the template as it appears. The part that matters most is the list of
platforms you actually tested on — network behaviour is not portable. Discovery
and mDNS work differently on Android than on desktop, and permissions change
what a scan can see.

## Licensing

By opening a pull request you agree that your contribution is offered under the
same license as the repository it lands in — Apache-2.0 for `vernet` and
`network_tools_flutter`, BSD-3-Clause for `network_tools`.
