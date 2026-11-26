# winget-apps2samsung

This repository is no longer in use.

It used to build the Windows installer (`.msi`) of
[Apps2Samsung](https://github.com/Apps2Samsung/Apps2Samsung) and submit each stable release to
WinGet. Both now happen in the Stable Release workflow of the main repository, where the
installer is also code signed:

- Installer definition: [`installer/Product.wxs`](https://github.com/Apps2Samsung/Apps2Samsung/blob/beta/installer/Product.wxs)
- Workflow: [`stable-release.yml`](https://github.com/Apps2Samsung/Apps2Samsung/blob/beta/.github/workflows/stable-release.yml), jobs `windows` and `winget`

Installing is unchanged:

```
winget install Apps2Samsung.Apps2Samsung
```

The `manifests` folder holds the WinGet manifests up to version 3.3.1, kept for reference. The
current ones are in [microsoft/winget-pkgs](https://github.com/microsoft/winget-pkgs/tree/master/manifests/a/Apps2Samsung/Apps2Samsung).
