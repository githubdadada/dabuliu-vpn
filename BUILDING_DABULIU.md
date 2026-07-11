# Building Dabuliu VPN

The app is a GPL-3.0 derivative of FlClash and retains the upstream license.

## Supported targets

- Android: `dart setup.dart android --env stable`
- macOS: `dart setup.dart macos --env stable`
- Windows: `dart setup.dart windows --env stable`

Flutter `3.44.6`, Go, platform build tools, and recursive Git submodules are
required. Windows must be built on Windows; macOS must be built on a Mac with
the full Xcode application installed.

The included `dabuliu-build.yml` workflow builds all three platforms on their
native GitHub Actions runners and uploads the packages as workflow artifacts.

## User onboarding

Do not embed a shared VPN password in the application. In 3X-UI, create or
select the user and copy the Clash subscription URL in this form:

```text
https://vpn.dabuliuai.top:2096/clash/<user-sub-id>
```

Import that URL in Dabuliu VPN. Each user then remains independently
meterable, expirable, and revocable from the management panel.
